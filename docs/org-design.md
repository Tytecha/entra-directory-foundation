# Northwind Services: Directory Design

## Group Design

I organized Northwind’s directory using Security groups with Assigned
membership. Group names follow SEC-<Type>-<Name>. Each group has a
description identifying its members and who approves membership changes.

| Group | Why it exists |
|---|---|
| SEC-Dept-Executive | Organizes the owner’s Executive department membership. |
| SEC-Dept-IT | Organizes staff responsible for technical operations and support. |
| SEC-Dept-Finance | Organizes staff responsible for payroll and invoicing. |
| SEC-Dept-Sales | Organizes the sales team, including the sixteenth Northwind user. |
| SEC-Dept-HR | Organizes staff responsible for employee onboarding and offboarding. |
| SEC-Role-Onboarding | Brings designated HR and IT staff together by shared responsibility. |
| SEC-Role-Contractor | Identifies contractors separately from employees. |

These groups establish a membership structure. They have not been
assigned application access in this lab.

## Why Departments and Their Limits

Departments provide a clear starting point because people in the same
team often need similar access. Adding the fifth salesperson required
creating an account and adding it to SEC-Dept-Sales.

Department membership alone becomes insufficient when teammates need
different permissions or people across departments perform the same
function. SEC-Role-Onboarding addresses the second case. Sensitive
access would need more specific groups and approval requirements.

## Contractor Decision

I placed contractors in SEC-Role-Contractor and excluded them from
employee department groups by default. Contractor status does not
justify access to employee resources. Any additional membership would
require an approved business need.

Contract end dates must be recorded and reviewed. Assigned group
membership does not expire automatically, so removal and account
disablement require a deliberate offboarding process.

## Scaling to 500 People

At 500 people, I would introduce automated onboarding and offboarding,
consistent department and job attributes, and regular membership
reviews. With appropriate licensing, I would consider dynamic
department groups and group-based application assignments.

I would retain role-based groups for shared responsibilities and use
separate approvals for sensitive access. Each group would have an
accountable owner to prevent unnecessary or outdated memberships.

## What I Changed During the Lab

My initial plan omitted an Executive group because an earlier
instruction discouraged single-member groups. A later instruction
required a group for every department, so I added SEC-Dept-Executive
and documented it as an exception.

This taught me to check requirements for conflicts and explain design
exceptions rather than silently changing the directory.
