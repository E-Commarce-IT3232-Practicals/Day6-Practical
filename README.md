# Employee Management System - Day06 (2025-04-11) 👨‍💼

## 📖 Overview

This is a **Java-based Employee Management System** built using **Spring Boot** and **Jakarta Persistence API (JPA)**. It allows you to manage relationships between employees, departments, projects, and insurance details seamlessly.

---

## 🏗️ Project Structure

### 🔹 Entity Models

The system includes four primary entities:

- **👨‍💼 Employee**
  - Attributes: `empNo`, `name`, `age`, `salary`, `gender`
  - Relationships:
    - 🔁 Many-to-One with `Department`
    - 🔁 Many-to-Many with `Project`
    - 🔁 One-to-One with `Insurance`

- **🏢 Department**
  - Attributes: `id`, `name`, `established`
  - Relationships:
    - 🔁 One-to-Many with `Employee`

- **💼 Project**
  - Attributes: `id`, `name`, `totalCost`
  - Relationships:
    - 🔁 Many-to-Many with `Employee`

- **🛡️ Insurance**
  - Attributes: `id`, `type`
  - Relationships:
    - 🔁 One-to-One with `Employee`

---

## 🔗 Entity Relationships

- 👨‍💼 An **employee** belongs to one **department**, but a **department** can have many **employees**.
- 👨‍💼 An **employee** can work on many **projects**, and each **project** can have many **employees**.
- 🛡️ An **employee** can have one **insurance** policy.

---

## 🛠️ Technologies Used

- ☕ **Java**
- 🌐 **Jakarta Persistence API (JPA)**
- 🧰 **Spring Boot**
- 🐬 **MySQL** (or your preferred RDBMS)

---

## 🧩 Database Schema

The application manages the following tables:

* `employee` 👨‍💼
* `department` 🏢
* `project` 💼
* `employee_project` 🔁 (join table)
* `insurance` 🛡️

---

## 🚀 Outputs

![Screenshot 1](https://github.com/user-attachments/assets/7dce511f-08b4-44d3-ac2e-96247fcd6639)
![Screenshot 2](https://github.com/user-attachments/assets/26c52822-091c-4a74-8fd9-9e001d08dd78)
