# Project Documentation

## 1. Project Overview

The Healthcare Practice Operations Tracking & Reporting System is an independent Google Sheets prototype designed to organise operational records and support management reporting for a simulated small healthcare practice operating across Abuja, Nigeria, and the United Kingdom.

The project focuses on structuring operational data before building reports and dashboards.

**Tools:** Google Sheets, spreadsheet formulas, data validation, conditional formatting, and charts.

**Data:** Synthetic data created for demonstration purposes only.

## 2. Project Objectives

- Organise related healthcare operational records into a structured workbook.
- Connect records using unique identifiers and reference fields.
- Automate routine calculations and status classifications.
- Track enquiries, follow-ups, appointments, inventory movements, and financial transactions.
- Summarise operational information through a management dashboard.

## 3. Workbook Architecture

The workbook contains 14 tabs organised into four functional groups.

### Foundation
- Patients
- Partners
- Next of Kin
- Providers
- Reference Lists

### Patient Acquisition & Service Delivery
- Enquiries
- Enquiry Follow-up
- Scheduling
- Appointments
- Appointment Follow-up

### Operational Resources & Finance
- Medical Supplies
- Inventory Transactions
- Financial Transactions

### Management Insight
- Management Reporting

## 4. Data Structure and Relationships

Unique identifiers and reference fields connect related records across the workbook.

- Partner and next-of-kin records reference patients.
- Enquiries and follow-up records support tracking contact history and outcomes.
- Scheduling records represent provider availability, while appointment records represent actual bookings.
- Inventory transactions record stock movements, allowing current stock to be calculated.
- Financial transactions record revenue and expenses, with optional patient and appointment references.

## 5. Automation and Data Quality

The prototype uses spreadsheet formulas and built-in features to reduce repetitive work and support consistency.

Examples include:
- Automated identifiers and calculated fields.
- Lookups for related information.
- Conditional calculations and status classifications.
- Summary calculations using counting and summation formulas.
- Dynamic inventory alerts.
- Dropdown validation and conditional formatting.

During testing, a financial summary initially returned zero because a transaction type contained a trailing space. Correcting the value restored the expected result and demonstrated the importance of data standardisation.

## 6. Reporting

The management dashboard includes:
- Patient and enquiry summary metrics.
- Appointment status reporting.
- Revenue by service.
- Revenue by location.
- Enquiries by source.
- Inventory alerts for low stock and restocking needs.

### Currency consideration

The simulated practice operates across Nigeria and the United Kingdom. Nigerian transactions use naira (NGN), while UK transactions use pounds sterling (GBP). These amounts should not be combined as directly comparable values without an explicit currency-conversion method.

Currency-aware reporting remains an area for refinement.

## 7. Limitations and Future Improvements

This is a portfolio prototype, not a production-ready electronic health record system or validated financial reporting platform.

Potential improvements include:
- Currency-aware financial reporting.
- Additional operational KPIs and trend analysis.
- More detailed enquiry conversion and appointment outcome analysis.
- A formal data dictionary.
- Further automation where appropriate.

Any real-world deployment would require proper assessment of data protection, access controls, auditability, backup procedures, and clinic-specific workflows.

## 8. Privacy and Scope

All demonstration records should be synthetic. No real patient information is required or intended for this project.

The prototype demonstrates data organisation and reporting concepts; it does not replace clinical judgement or a dedicated clinical information system.
