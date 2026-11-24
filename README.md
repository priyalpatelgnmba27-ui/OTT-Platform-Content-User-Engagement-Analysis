# StreamSphere OTT Platform: Content & User Engagement Analysis using PostgreSQL

**MBA End-Term Project | SQL and Data Management (PMDE30605)**  
**IILM University, Greater Noida**

## 1. Project Overview

StreamSphere is a hypothetical OTT (Over-The-Top) streaming platform designed for this academic project. This project focuses on analysing content performance, user engagement, subscription trends and payment activities using PostgreSQL.

The project integrates six separate CSV datasets into a relational database, performs data cleaning and validation, and uses SQL queries to generate meaningful business insights.

The analysis helps understand viewer preferences, content popularity, subscription performance, revenue collection and potential business risks.

## 2. Project Objectives

- Design a relational database and ER diagram for an OTT platform.
- Create and manage tables using PostgreSQL.
- Implement primary keys, foreign keys and CHECK constraints.
- Identify and clean data quality issues.
- Analyse content performance and user engagement.
- Evaluate subscription plans and payment performance.
- Use advanced SQL queries to generate business insights.
- Demonstrate database integrity and transaction management.

## 3. Technologies Used

- **Database:** PostgreSQL 16
- **Database Management Tool:** pgAdmin 4
- **Query Language:** SQL
- **Data Format:** CSV
- **Analysis Techniques:** Joins, Aggregations, Subqueries, CTEs, Window Functions and Date Functions
- **Visualisation:** Python (Matplotlib)

## 4. Dataset Description

The project uses a hypothetical dataset containing six related tables and a total of 1,270 records.

| Dataset | Description | Records |
|---|---|---:|
| Users | User details, age, city and signup date | 100 |
| Content | Movies, series, documentaries and genres | 40 |
| Subscriptions | Subscription plans, prices and status | 115 |
| Viewing History | Viewing sessions, watch minutes and completion | 600 |
| Ratings | User ratings and rating dates | 300 |
| Payments | Payment amounts, methods and statuses | 115 |
| **Total** | | **1,270** |

A data dictionary is also included to explain the dataset columns.

**Note:** The dataset is hypothetical and was prepared for this academic project. It does not represent actual customer data from a real OTT company.

## 5. Database Design

The database consists of six interconnected tables:

- `users`
- `content`
- `subscriptions`
- `viewing_history`
- `ratings`
- `payments`

Primary keys and foreign keys establish relationships between tables. CHECK constraints help maintain valid data, while indexes support database operations.

## 6. Project Workflow and SQL Implementation

The SQL project is organised into the following sections:

| Section | Description |
|---|---|
| 1 | Table creation, keys, constraints and indexes |
| 2–3 | Table verification and data loading |
| 4–6 | Data quality checks, cleaning and verification |
| 7 | Ten business analysis queries |
| 8 | Data integrity and revenue risk audit |
| 9 | Constraint testing using invalid insert attempts |
| 10 | Transaction management using COMMIT, ROLLBACK and SAVEPOINT |

SQL concepts used include:
- SELECT, WHERE and ORDER BY
- INNER JOIN and other joins
- GROUP BY and aggregate functions
- CASE statements
- Subqueries and CTEs
- RANK() window function
- DATE_TRUNC() date function

## 7. Key Business Findings

The analysis generated the following insights:

- Movies represent 17 out of 40 titles but contribute **57.9% of total watch minutes**.
- Series have a higher completion rate of **73.6%**, compared with **64.0%** for movies.
- *Midnight Run* is the most-watched title but has the lowest average rating of **1.91**.
- Premium and Standard plans together contribute **77% of revenue**.
- The Standard plan has the highest cancellation rate of **27.6%**.
- **₹7,980 (18.2% of billed value)** is in failed or pending payments.

## 8. Business Recommendations

1. Improve payment recovery through automatic retries and timely follow-ups.
2. Reduce Standard plan cancellations through retention offers and flexible subscription options.
3. Consider viewer ratings along with watch time when promoting content.
4. Review content categories and invest in genres with strong engagement.
5. Use user engagement segments to develop personalised recommendations.
6. Strengthen data governance through regular validation and integrity checks.

## 9. Repository Structure

```text
OTT-Platform-Content-User-Engagement-Analysis/
│
├── README.md
│
├── data/
│   ├── users.csv
│   ├── content.csv
│   ├── subscriptions.csv
│   ├── viewing_history.csv
│   ├── ratings.csv
│   ├── payments.csv
│   └── data_dictionary.csv
│
├── sql/
│   └── streamsphere_project.sql
│
└── report/
    └── StreamSphere_Project_Report.pdf
```

## 10. How to Run the Project

1. Install PostgreSQL and open pgAdmin 4.
2. Create a database named `streamsphere`.
3. Open the Query Tool for the newly created database.
4. Execute Section 1 of `streamsphere_project.sql` to create the tables and indexes.
5. Import the six CSV files into their respective tables in the following order:
   - users
   - content
   - subscriptions
   - viewing_history
   - ratings
   - payments
6. Execute the remaining SQL script from Section 2 onwards.
7. Review the query outputs, data quality checks and business insights.

## 11. Project Team

**Submitted By:**

1. Shruti Saraswat
2. Khushi Sharma
3. Vashvi Gupta
4. Harshit Shukla
5. Priyal Patel

**Faculty Guide:** Dr. Lalit Kumar  
**Institution:** IILM University, Greater Noida  
**Course:** SQL and Data Management (PMDE30605)  
**Project Type:** MBA End-Term Group Project  
**Submission Date:** 25 November 2026

## 12. Individual Contribution – Priyal Patel

My key responsibilities in this project included:

- Performing database integrity tests to check data validity and consistency.
- Demonstrating transaction management using COMMIT, ROLLBACK and SAVEPOINT.
- Identifying business risks related to payment failures and subscription cancellations.
- Developing business recommendations based on SQL analysis results.
- Contributing to project report preparation and presentation development.

**Key Learning:** Gained practical understanding of PostgreSQL, database integrity, transaction management and SQL-based business decision-making.

## 13. Conclusion

This project demonstrates how PostgreSQL can transform separate datasets into a structured relational database and support business decision-making through SQL analysis. It provides insights into content performance, viewer engagement, subscription cancellations and payment risks while demonstrating database design, data cleaning, integrity constraints and transaction management.

---

**References**

- PostgreSQL Official Documentation: https://www.postgresql.org/docs/16/
- Chen, P. P. (1976). The Entity-Relationship Model: Toward a Unified View of Data.
- Elmasri, R., & Navathe, S. (2016). Fundamentals of Database Systems (7th Edition).
