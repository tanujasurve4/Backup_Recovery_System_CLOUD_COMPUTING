# ☁️ Backup and Recovery System Using S3

A cloud-based backup and recovery system developed using **Amazon S3** to securely store, automatically backup, and recover files whenever required.

---

## 📌 Project Overview

Traditional file storage systems often depend on manual backups, making recovery slow and unreliable.

This project uses **Amazon S3** to provide secure cloud storage with automatic backup and quick file recovery using a primary and backup S3 bucket.

---

## 🎯 Objectives

- ☁️ Store files securely in Amazon S3.
- 💾 Automatically backup uploaded files.
- 🔄 Restore files quickly from backup storage.
- 🔐 Provide secure user authentication.
- 🕐 Maintain file versions using S3 Versioning.
- 🛡️ Reduce the risk of data loss.

---

## ✨ Key Features

- 👤 User Registration & Login
- 📤 Upload Files
- 👁️ View Files
- 🗑️ Delete Files
- ☁️ AWS S3 Cloud Storage
- 💾 Automatic Backup to Secondary S3 Bucket
- 🔄 File Recovery / Restore
- 🕐 S3 Versioning
- 🔐 AWS IAM Access Control

---

## 🛠️ Technologies Used

- HTML5
- CSS3
- Bootstrap
- JavaScript
- JSP
- Java Servlets
- JDBC
- MySQL
- Amazon S3
- AWS IAM
- Amazon EC2
- Apache Tomcat

---

## 🏗️ System Architecture

```text
             👤 User
                │
                ▼
       ┌─────────────────┐
       │  JSP / HTML /   │
       │ CSS / JavaScript│
       └────────┬────────┘
                │
                ▼
       ┌─────────────────┐
       │  Java Servlets  │
       │      MVC        │
       └──────┬─────┬────┘
              │     │
              ▼     ▼
          MySQL   AWS S3
                    │
             ┌──────┴──────┐
             ▼             ▼
        Primary S3     Backup S3
          Bucket         Bucket
             │             │
             └──── Restore ┘
