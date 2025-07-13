# 🛡️ WeLearnSecShop Docker Lab

A vulnerable e-commerce web application designed for practicing web application penetration testing and bug bounty techniques. This setup uses Docker to simulate a realistic lab environment with minimal system resource usage — no need to run a full Virtual Machine.

---

## 📦 Components

This lab environment includes:

- `welearnsecshop`: A vulnerable PHP web application (cloned from [WeLearnSec GitHub](https://github.com/welearnsec/welearnsecshop))
- `MariaDB`: MySQL-compatible database server
- `phpMyAdmin`: Web-based MySQL DB management at `localhost:8087`

---

## 🚀 Getting Started

### 1️⃣ Start the lab environment

Run the following command from the project directory:

```bash
docker-compose up --build

To reset the lab environment:

```bash
docker-compose down -v

## 📝 Additional Notes

### 📁 Directory Structure

After downloading this repository, make sure to clone the welearnsecshop project into the same directory. The expected folder structure is:

```bash
.
├── config/
│   └── apache.conf
├── Dockerfile
├── docker-compose.yml
└── welearnsecshop/
```

To clone vulnerable app:
```bash
git clone https://github.com/welearnsec/welearnsecshop

### 🌐 Access the Application

The vulnerable app will be accessible at:

```bash
http://localhost:8086

PHPMyAdmin creds can be found at docker-compose.yml file.

## 🙏 Credits

- Vulnerable app by WeLearnSec
- Docker environment by damienmagdangal