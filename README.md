# IT Asset Management Database (Oracle SQL & PL/SQL)

## Project Overview

A production-oriented **IT Asset Management (ITAM) relational database** using Oracle SQL and PL/SQL. It focuses on designing, securing, migrating, and optimizing enterprise-grade databases that support real business workflows such as asset tracking, auditing, and operational reporting.

The work emphasizes data integrity, automation, cloud migration readiness, and performance tuning, mirroring responsibilities commonly found in enterprise IT, cloud infrastructure, and platform engineering roles.

## Why This Project Matters

Enterprise systems depend on reliable, secure, and performant databases. Poor schema design, missing constraints, or inefficient queries can directly impact uptime, security, and cost.

This project demonstrates:
- How to model business-critical data using relational design best practices
- How to enforce correctness and consistency at the database layer
- How to automate operational logic with PL/SQL instead of relying solely on application code
- How to prepare and migrate databases for cloud environments
- How to analyze and optimize query performance under realistic workloads

These are foundational skills for cloud engineers, platform engineers, and backend developers working in regulated or enterprise-scale environments.

## Core Capabilities & Exercises

### Business-Driven Query Design
Developed SQL queries to support real business questions such as asset utilization, ownership tracking, and inventory status.

- Complex `SELECT` statements
- Multi-table `JOIN`s
- Aggregations, filtering, grouping, and ordering
- Query readability and maintainability

### Cloud Migration & User Management
Migrated the ITAM database to **Oracle Cloud**, simulating an enterprise transition from on-prem to cloud infrastructure.

- Schema migration
- User creation and role-based access control
- Separation of duties and least-privilege access

### Data Integrity & Relational Enforcement
Implemented robust constraints to ensure long-term data correctness and prevent invalid states.

- `PRIMARY KEY`, `FOREIGN KEY`
- `UNIQUE`, `CHECK`, `NOT NULL`
- Referential integrity across asset and user tables

### Database Automation with PL/SQL
Automated business logic directly at the database layer to improve reliability and reduce application complexity.

- User-defined functions
- Stored procedures
- Triggers for lifecycle events
- Reduction of manual and repetitive operations

### Performance Tuning & Optimization
Analyzed and improved database and query performance using Oracle tooling and indexing strategies.

- Index design and trade-offs
- Execution plan analysis
- Query refactoring for efficiency
- Performance considerations for scaling systems

## Architecture & Database Resources

Included design artifacts and schema documentation to support maintainability and knowledge transfer:


- SQL scripts to create ITAM and Murach reference tables
- Clear separation between schema creation, constraints, and procedural logic
- IT Asset Management ER Diagram
![diagram](/diagrams/ITAssetMgmnt_Diagram.png)
- AP Schema Diagram
![diagram](/diagrams/ap_schema.png)


## Tech Stack

| Layer | Technology |
| --- | --- |
| **Database** | Oracle Database |
| **Query Language** | SQL |
| **Procedural Logic** | PL/SQL |
| **Tooling** | Oracle SQL Developer |
| **Cloud** | Oracle Cloud Infrastructure (OCI) |
| **Concepts** | Data Integrity, RBAC, Automation, Performance Tuning |

## Repository Structure

```text
├── student_create_itam/
│   └── ITAM schema creation scripts
├── create_Murach_tables/
│   └── Reference tables and sample datasets
├── diagrams/
│   ├── ITAssetMgmnt_Diagram.png
│   └── ap_schema.png
├── plsql/
│   ├── ex3.sql
│   ├── ex4.sql
│   ├── ex5.sql
│   ├── ex6.sql
│   ├── ex7.sql
└── README.md
```

## Key Takeaways

- Strong database design prevents entire classes of bugs before they reach application code
- Constraints and triggers are critical for defensive data engineering
- Cloud migration requires planning around users, roles, and security, not just schemas
- Performance tuning is an iterative, measurement-driven process
- Databases remain a core pillar of cloud-native and enterprise systems

## References

- Murach’s Oracle SQL and PL/SQL for Developers (2nd Edition) - Joel Murach
- Oracle SQL Developer Documentation
- Oracle Cloud Infrastructure Database Guides
