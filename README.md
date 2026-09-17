# Hi there 👋

I'm a Software Engineer at **HedgeSPA**, a fintech company in Hong Kong, building production systems with **Java**, **Spring Boot**, **React/TypeScript**, and **SQL**. I focus on backend architecture, data correctness under concurrency, and full-stack ownership of complex, stateful features.

---

## 🚀 About Me
- Full-stack engineer working across Java/Spring Boot backends and React/TypeScript frontends in production fintech systems
- Comfortable owning a feature end-to-end: data model, business logic, REST API, and UI
- Experience designing systems where correctness under concurrency matters — optimistic locking, distributed session management, and reconciliation invariants
- Built and shipped a multi-tab financial calculation module independently, from a formal spec, in under 3 weeks
- Contributor to open-source Java tooling (springwolf-core, openapi-generator)
- Comfortable working with Git-based workflows, CI/CD pipelines, and API testing with Postman

---

## 💻 Tech Stack:
![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white) ![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white) ![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white) ![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB) ![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E) ![Redis](https://img.shields.io/badge/redis-%23DD0031.svg?style=for-the-badge&logo=redis&logoColor=white) ![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white) ![Solidity](https://img.shields.io/badge/Solidity-%23363636.svg?style=for-the-badge&logo=solidity&logoColor=white) ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![Bootstrap](https://img.shields.io/badge/bootstrap-%238511FA.svg?style=for-the-badge&logo=bootstrap&logoColor=white) ![jQuery](https://img.shields.io/badge/jquery-%230769AD.svg?style=for-the-badge&logo=jquery&logoColor=white) ![NPM](https://img.shields.io/badge/NPM-%23CB3837.svg?style=for-the-badge&logo=npm&logoColor=white) ![Thymeleaf](https://img.shields.io/badge/Thymeleaf-%23005C0F.svg?style=for-the-badge&logo=Thymeleaf&logoColor=white) ![Apache Tomcat](https://img.shields.io/badge/apache%20tomcat-%23F8DC75.svg?style=for-the-badge&logo=apache-tomcat&logoColor=black) ![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white) ![SQLite](https://img.shields.io/badge/sqlite-%2307405e.svg?style=for-the-badge&logo=sqlite&logoColor=white) ![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white) ![MicrosoftSQLServer](https://img.shields.io/badge/Microsoft%20SQL%20Server-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white) ![GitLab CI](https://img.shields.io/badge/gitlab%20CI-%23181717.svg?style=for-the-badge&logo=gitlab&logoColor=white) ![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white) ![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white) ![GitLab](https://img.shields.io/badge/gitlab-%23181717.svg?style=for-the-badge&logo=gitlab&logoColor=white) ![Jira](https://img.shields.io/badge/jira-%230A0FFF.svg?style=for-the-badge&logo=jira&logoColor=white) ![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)

---

## 📌 Featured Work

### 🔹 Financial Calculation Module (HedgeSPA)
Independently designed and shipped a 5-tab financial calculation module from a formal spec in under 3 weeks. Covers a multi-entity data model, a transaction lifecycle with pending/confirmed states, and a valuation engine enforcing tolerance-checked reconciliation invariants to 6 decimal places. Includes a sequencing-sensitive pricing step that separates pre-transaction snapshots from post-transaction recomputation to prevent value dilution.

### 🔹 Distributed Session Management (HedgeSPA)
Designed a Redis-backed concurrent session detection system with silent JWT refresh via Axios interceptors, OTP-based registration, and an inactivity keepalive mechanism. Diagnosed and fixed a scheduler defect that was silently invalidating active sessions by keying cleanup off the wrong token's expiry.

### 🔹 Transaction Processing & Validation Engine (HedgeSPA)
Architected a rules-based transaction engine with separated draft and committed states, partial-edit REST endpoints, and optimistic locking with retry logic on shared counters. Built a companion date-aware validation engine that conditionally applies rule sets based on entity history, replacing a hardcoded limit with a configurable window.

### 🔹 Multi-Tenant Billing System (HedgeSPA)
Delivered a multi-tenant onboarding and subscription billing system end-to-end: schema design, role/tier-based access controls, plan upgrade workflow, quota enforcement with optimistic locking, and default-config auto-provisioning for new signups.

### 🔹 Open Source Contributions
Found and fixed a null-pointer bug in [springwolf-core](https://github.com/springwolf/springwolf-core)'s `SwaggerSchemaMapper`: composed schemas (`allOf`/`oneOf`/`anyOf`) with no explicit type were crashing `Set.of()`, silently dropping channels and operations from the generated AsyncAPI docs. Fix + regression test merged in [PR #1835](https://github.com/springwolf/springwolf-core/pull/1835). Currently scoped on a fix for [openapi-generator](https://github.com/OpenAPITools/openapi-generator) (Issue #24686), a widely-used OpenAPI code generation tool.

### 🔹 Event Management System (Spring Boot + Oracle SQL)
[🔗 View Repository](https://github.com/itsmib/event-management-system)
Full-stack ticketing and event platform with OTP-based registration, role-gated access across 8+ screens, seat reservation logic, and live payment processing via Razorpay, backed by a normalized schema across 12+ tables.

### 🔹 Car Rental System
[🔗 View Repository](https://github.com/itsmib/Car-Rental-System)
A Java-based application for managing car rentals. Automates booking, customer management, and rental transaction tracking, built for reliability and easy maintenance.

### 🔹 Crime Reporting & Analysis System
[🔗 View Repository](https://github.com/itsmib/Crime-Reporting-Analysis-System)
A Java-based system designed to facilitate crime reporting and basic analysis. Enables users to report incidents, and provides tools to analyze trends in crime data.

### 🔹 FlexBox Playground
[🔗 View Repository](https://github.com/itsmib/Flexbox-PlayGround)
Interactive resource for experimenting with CSS Flexbox layouts and responsive design patterns.

### 🔹 Library Management System
[🔗 View Repository](https://github.com/itsmib/Library-Management-System)
Python-based library management tool integrating MySQL for book, member, and transaction management.

---

## 🌐 Socials:
[![Instagram](https://img.shields.io/badge/Instagram-%23E4405F.svg?logo=Instagram&logoColor=white)](https://instagram.com/its.mib) [![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://linkedin.com/in/itsmib) [![Stack Overflow](https://img.shields.io/badge/-Stackoverflow-FE7A16?logo=stack-overflow&logoColor=white)](https://stackoverflow.com/users/31984259) [![email](https://img.shields.io/badge/Email-D14836?logo=gmail&logoColor=white)](mailto:noorulmisbah15@gmail.com)

---

⭐ _Thanks for visiting — feel free to explore the repositories and reach out._

---
[![](https://visitcount.itsvg.in/api?id=itsmib&icon=0&color=0)](https://visitcount.itsvg.in)
