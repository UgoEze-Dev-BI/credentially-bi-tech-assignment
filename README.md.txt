# Credentially BI Tech Assignment

## 📊 Project Overview

This Power BI dashboard provides a detailed overview of the candidate reference process at Credentially. It is designed to help hiring teams monitor the progress, speed, and approval outcomes of reference requests across different job positions and assigned recruiters.

## ✅ Objectives Addressed

The dashboard tracks the full reference lifecycle from Requested to Submitted and then Approved or Declined. It calculates the average time taken to complete a reference and provides insights broken down by job role, reference status, and the user responsible for the job position. The solution is built on a cleaned and optimized semantic model using the provided data sources.

## 📁 Data Used

The dashboard connects to five main tables: `ref_references`, `ref_job_positions`, `ref_assigned_to`, `ref_user_tags`, and a calculated `Dates` table. Relationships were reviewed and cleaned to avoid many-to-many joins, with a central star-schema structure built around `ref_job_positions`.

## 📌 Key Metrics

The report includes metrics such as total reference count, number of submitted, approved, and declined references, approval rate percentage, and the average days from request to completion. These are supported by visual trends to monitor progress over time.

## 🎨 Features

The dashboard presents a clean, one-page layout with key performance indicators at the top and visuals arranged for intuitive analysis. Users can interact with slicers for Year, Month, Reference Approval Status, Role, and Assigned To. Reference trends and lifecycle visuals help stakeholders quickly identify bottlenecks or inefficiencies. A completion time chart with conditional formatting highlights turnaround speed.

## 🔐 GDPR & Data Privacy

The dashboard includes an "Assigned To" slicer, which references internal users responsible for managing reference requests. This is considered personal or semi-personal data under GDPR. For internal use, this data is appropriate, but access must be restricted to authorized users only. In public-facing or external contexts, the assigned_to field should be anonymized or aggregated. Future enhancements may include implementing Row Level Security (RLS) to control visibility based on user role or login. No candidate PII (personally identifiable information) is used or exposed.

## 🛠 Tools Used

This dashboard was developed in Power BI Desktop using Power Query for data shaping and DAX for custom metrics and time intelligence. It incorporates a theme file and semantic model components provided in the assignment.

## 🚀 How to Use

Open the file `Credentially_References_Dashboard.pbix` in Power BI Desktop. Use the slicers to filter by year, month, reference status, role, or assigned recruiter. Hover over visuals to see tooltips for deeper insights. Use the trend visuals and completion time metrics to identify slow references and improve hiring process speed.

---

Submitted by: Ugo Ezeli 
Repository: https:https://github.com/UgoEze-Dev-BI/credentially-bi-tech-assignment
