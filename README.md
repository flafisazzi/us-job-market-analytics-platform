# 📄 Business Requirements Document (BRD)
## Project Name: AI-Driven Career Analytics & Resume Optimization System  
**Version:** 1.0  
**Author:** Flavia Azzi Nasser  
**Date:** July 2, 2026  

---

## 1. Project Overview & Context
The data professional job market in the United States demands aggressive resume customization to successfully pass through Applicant Tracking Systems (ATS) and align with distinct employment contracts (W2, C2C, Direct Hire). Tracking conversions manually causes severe data fragmentation. This project establishes an enterprise-grade Analytics infrastructure to track the end-to-end recruitment funnel, audit resume version performance, and plan cloud-scale database migration.

---

## 2. Stakeholder Interview Transcript (Simulated)
* **Interviewer:** Data Analytics Portfolio Lead
* **Stakeholder:** Job Market Candidate (Business Owner / Core User)

> **Interviewer:** What is the primary business problem we are trying to solve?
> **Stakeholder:** I need to manage my job applications in the US market, but more importantly, I need data-driven proof of *which* version of my resume works best. I tailor my job titles, professional summaries, and technical skills to the Job Description. Right now, I don't know if my Power BI resume or my Data Engineer resume converts more interviews.
> 
> **Interviewer:** What channels and metrics are critical for your daily operations?
> **Stakeholder:** I need to track the job origin (LinkedIn, Dice, ZipRecruiter, Referrals) and the exact method of engagement (Phone Call, Email, Portal Registration). For metrics, I need overall application volume, conversion/success rates of active leads, rejection rates, and annualized average salary—converting W2 hourly rates ($/hr * 2080 hours) to compare them fairly with Direct Hire annual salaries.
> 
> **Interviewer:** What is the technical vision for this platform?
> **Stakeholder:** We will start with a local Excel relational model to build a Fast MVP and design the initial Power BI dashboard. Once validated, we must design the schemas to migrate this infrastructure into a Cloud Environment using Azure SQL or Databricks Delta Tables to show cloud architecture capabilities.

---

## 3. Business & Technical Requirements
* **BR-01:** The system must track the recruitment funnel stages (Applied, Resume Sent, Initial Contact, RTR Submitted, Interview, Rejected/Closed).
* **BR-02:** Every application must be strictly linked to a specific resume version ID to analyze profile performance.
* **BR-03:** Hourly W2 contract compensation must be annualized using the standard 2,080-hour multiplier.
* **TR-01:** Data architecture must use clean `Snake_Case` formatting across all tables to ensure compatibility with Azure SQL and Databricks Spark SQL.
* **TR-02:** Power BI model must follow a strict Star Schema (1:N relationships) avoiding flat-table architectures.

---

## 📅 4. Project Schedule & Milestones

| Phase | Milestone / Task | Estimated Duration | Target Finish Date | Deliverable |
| :--- | :--- | :--- | :--- | :--- |
| **Phase 1** | Requirements & Documentation | 3 Days | July 05, 2026 | Word BRD & GitHub Repository Setup |
| **Phase 2** | Relational Data Modeling (Excel) | 4 Days | July 09, 2026 | Normalized Excel Database (Star Schema) |
| **Phase 3** | Power BI MVP & DAX Engineering | 5 Days | July 14, 2026 | Local Power BI Dashboard Prototype |
| **Phase 4** | Cloud Migration Architecture Plan | 4 Days | July 18, 2026 | SQL DDL Scripts / Databricks Delta Schema |
| **Phase 5** | GitHub Portfolio Deployment | 2 Days | July 20, 2026 | Production README.md & Final Project Sign-off |
