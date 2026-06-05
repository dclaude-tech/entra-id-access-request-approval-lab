# IAM Access Request and Approval Lab | Microsoft Entra ID

## Overview

This project is a hands-on IAM lab built in Microsoft Entra ID to simulate access request and approval workflows.

I used this project to practice how an IAM Analyst may review access requests, validate business justification, route approvals, verify access assignments, and document ticket closure.

The goal was to build a realistic request workflow using fictional users, security groups, access packages, and ticket scenarios in a controlled lab environment.

## Scenario

Northstar Identity Lab is a fictional organization with department-based access needs across Finance, HR, and IT.

In this lab, users request access to specific resources through Microsoft Entra entitlement management. Each request is reviewed based on least privilege, business need, approval requirements, and verification evidence.

## What this lab demonstrates

This lab demonstrates how access requests can be handled from intake to closure, including:

* Creating access groups for department resources
* Creating fictional lab users for request and approval scenarios
* Creating Microsoft Entra access packages
* Configuring request and approval policies
* Submitting access requests as fictional users
* Approving or denying requests based on business context
* Verifying access package assignments
* Verifying backing security group membership
* Documenting IAM ticket outcomes

## Lab environment

The lab uses a Microsoft Entra ID tenant named Northstar Identity Lab.

All users, groups, access packages, and tickets are fictional and created only for learning and portfolio documentation.

## Planned ticket workflows

| Ticket     | Access request                       | Planned outcome       |
| ---------- | ------------------------------------ | --------------------- |
| TICKET-001 | Finance reports read-only access     | Approved              |
| TICKET-002 | HR employee records read-only access | Denied                |
| TICKET-003 | IT service desk tools access         | Approved after review |

## Planned access model

| Resource area         | Access package              | Backing security group      |
| --------------------- | --------------------------- | --------------------------- |
| Finance reports       | AP-Finance-Reports-Read     | SG-Finance-Reports-Read     |
| HR employee records   | AP-HR-Employee-Records-Read | SG-HR-Employee-Records-Read |
| IT service desk tools | AP-IT-ServiceDesk-Tools     | SG-IT-ServiceDesk-Tools     |

## Skills practiced

* IAM access request review
* Approval workflow documentation
* Least-privilege decision making
* Microsoft Entra entitlement management
* Access package configuration
* Security group-based access assignment
* Access verification
* Access denial documentation
* IAM ticket documentation
* Evidence collection

## Repository structure

```text
screenshots/
tickets/
README.md
```

## Evidence plan

Screenshots will be collected throughout the lab to document the setup and workflow results.

Planned evidence includes:

* Repository setup
* Microsoft Entra security groups
* Fictional lab users
* Access packages
* Request and approval policies
* Submitted access requests
* Approval and denial decisions
* Access package assignments
* Security group membership verification
* Closed ticket documentation

## Project status

In progress.

## Important note

This is a fictional lab environment created for portfolio and learning purposes. It does not include confidential, employer, customer, or production information.
