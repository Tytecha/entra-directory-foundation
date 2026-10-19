# Northwind Services Directory Design

Name	Department	Job title	Planned groups
Morgan Reed	Executive	Owner / CEO	None — no executive group because there is only one member
Jordan Brooks	IT	IT Manager	SEC-Dept-IT
Avery Chen	IT	Systems Administrator	SEC-Dept-IT
Taylor Davis	IT	Help Desk Technician	SEC-Dept-IT
Angela Day	Finance	Finance Manager	SEC-Dept-Finance
Noah Patel	Finance	Payroll Specialist	SEC-Dept-Finance
Olivia Grant	Finance	Accounts Receivable Specialist	SEC-Dept-Finance
Ethan Wilson	Sales	Sales Manager	SEC-Dept-Sales
Sophia Martinez	Sales	Account Executive	SEC-Dept-Sales
Liam Thompson	Sales	Account Executive	SEC-Dept-Sales
Chloe Bennett	Sales	Sales Development Representative	SEC-Dept-Sales
Grace Lewis	HR	HR Manager	SEC-Dept-HR
Daniel Kim	HR	HR Coordinator	SEC-Dept-HR
Riley Parker	Contractors	Contract Project Coordinator	SEC-Role-Contractor
Cameron Ellis	Contractors	Contract Content Specialist	SEC-Role-Contractor

## Design Decisions

- Names and job titles are fictional lab data.
- Department groups organize employees by business department.
- Contractors belong to SEC-Role-Contractor.
- No group is created solely for the owner or the help desk technician.
- The owner has no planned group membership at this stage.
- Group membership alone does not grant Microsoft Entra administrator roles.

## User and Group Membership Plan
