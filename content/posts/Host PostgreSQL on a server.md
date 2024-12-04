---
title: Host PostgreSQL on a server
date: 2024-12-02
draft: false
tags:
  - database
  - server
---

## 🌐 **How to Host PostgreSQL on a Dedicated Server**

Learn how to set up and configure **PostgreSQL** on a dedicated Ubuntu server, and connect it to a **Node.js application**. This guide walks you through each step, from creating a server to installing PostgreSQL, setting up user access, and connecting with Node.js.
<!--more-->

---

## 🛠️ **PostgreSQL Setup Steps**

### **1. Create a Ubuntu Server**

Use any cloud platform to create a dedicated Ubuntu server.

### **2. Log in to the server using SSH**

```bash
ssh root@server_ip
```

### **3. Update the server**

Run the following commands to ensure your server is up-to-date:

```bash
sudo apt update
sudo apt upgrade
```

### **4. Install PostgreSQL**

Install PostgreSQL and its additional tools:

```bash
sudo apt install postgresql postgresql-contrib
```

### **5. Switch to the PostgreSQL user**

```bash
sudo su - postgres
```

### **6. Open the PostgreSQL shell**

```bash
psql
```

### **7. Set up the database and user**

Run the following commands inside the PostgreSQL shell:

```sql
-- Set a password for the PostgreSQL user
password postgres  

-- Create a new database
CREATE DATABASE mydb;

-- Create a new user
CREATE ROLE myuser WITH PASSWORD 'mypassword';

-- Grant privileges to the new user
GRANT ALL PRIVILEGES ON DATABASE mydb TO myuser;

-- Give superuser privileges to the new user
ALTER ROLE myuser WITH SUPERUSER;
```

### **8. Configure PostgreSQL to accept connections**

Find the configuration file:

```bash
sudo find / -name "postgresql.conf"
```

Edit the file:

```bash
sudo nano /path/to/postgresql.conf
```

Find the line:

```plaintext
#listen_addresses = 'localhost'
```

Uncomment it and change it to:

```plaintext
listen_addresses = '*'
```

### **9. Update access settings**

Find the access control file:

```bash
sudo find / -name "pg_hba.conf"
```

Edit the file to allow controlled access:

```bash
sudo nano /path/to/pg_hba.conf
```

Add this line at the end of the file:

```plaintext
host    all             all             0.0.0.0/0               md5
```

### **10. Restart PostgreSQL**

```bash
sudo service postgresql restart
```

---

## 🤝 **Connecting with Node.js**

### **11. Create a new directory for your Node.js project**

```bash
mkdir pg-db-connect
cd pg-db-connect
```

### **12. Initialize a new Node.js project**

```bash
npm init -y
```

### **13. Install the `pg` package**

```bash
npm install pg
```

### **14. Create a `database.js` file**

Add the following content:

```javascript
const { Pool } = require('pg');

const pool = new Pool({
    user: 'myuser',        // Replace with your username
    host: 'server_ip',     // Replace with your server IP
    database: 'mydb',      // Replace with your database name
    password: 'mypassword',// Replace with your password
    port: 5432,
});

module.exports = pool;
```

### **15. Create an `index.js` file**

Add the following content:

```javascript
const pool = require('./database');

async function createUserTable() {
    try {
        await pool.query(`CREATE TABLE IF NOT EXISTS users (
            id SERIAL PRIMARY KEY,
            name VARCHAR(50),
            age INTEGER
        )`);

        // Uncomment to insert a user
        // await pool.query(`INSERT INTO users (name, age) VALUES ($1, $2)`, ['Kunal', 18]);

        const result = await pool.query('SELECT * FROM users');
        console.log('Users:', result.rows);
    } catch (err) {
        console.error('Error creating user:', err);
    } finally {
        pool.end(); // Close the pool
    }
}

createUserTable();
```

### **16. Run the Node.js application**

```bash
node index.js
```

This will create the `users` table if it doesn't exist and display all users in the database.

---

## 🔒 **Pro Tips for Security**

1. **Keep your server updated** to protect against vulnerabilities.
2. **Do not expose sensitive information** like database credentials in public repositories.

---

You're now ready to host **PostgreSQL** on your server and connect it to a **Node.js application**! 🎉 Keep experimenting and building amazing projects! 🚀