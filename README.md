# IAM Access Request and Approval Lab | Microsoft Entra ID

## Overview

This project is a hands-on IAM lab built in Microsoft Entra ID to simulate access request and approval workflows.

I used this project to practice how an IAM Analyst may review access requests, validate business justification, route approvals, verify access assignments, and document ticket closure.

The goal was to build a realistic access request workflow using fictional users, security groups, access packages, and ticket scenarios in a controlled lab environment.

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

All users, groups, access packages, and tickets were created only for learning and portfolio documentation.

## Lab identities

| User          | Role in lab             | Workflow use                              |
| ------------- | ----------------------- | ----------------------------------------- |
| Ava Finance   | Finance requester       | Requests Finance reports read-only access |
| Mia HR        | HR requester            | Requests HR employee records access       |
| Leo IT        | IT requester            | Requests IT service desk tools access     |
| Riley Manager | Approver/resource owner | Reviews access requests                   |

The lab identities are fictional users created for access request and approval testing.

## Completed ticket workflows

| Ticket     | Access request                       | Outcome               |
| ---------- | ------------------------------------ | --------------------- |
| TICKET-001 | Finance reports read-only access     | Approved              |
| TICKET-002 | HR employee records read-only access | Denied                |
| TICKET-003 | IT service desk tools access         | Approved after review |

## Ticket documentation

| Ticket | Documentation | Summary |
|---|---|---|
| TICKET-001 | [TICKET-001 finance reports read](tickets/TICKET-001-finance-reports-read.md) | Approved Finance reports access request |
| TICKET-002 | [TICKET-002 HR employee records read](tickets/TICKET-002-hr-employee-records-read.md) | Denied HR employee records access request |
| TICKET-003 | [TICKET-003 IT service desk tools](tickets/TICKET-003-it-servicedesk-tools.md) | Approved IT service desk tools access request |

Each ticket documents the requester, requested access, business justification, IAM review notes, approval decision, verification results, evidence, and closure notes.

## Access model

| Resource area         | Access package              | Backing security group      |
| --------------------- | --------------------------- | --------------------------- |
| Finance reports       | AP-Finance-Reports-Read     | SG-Finance-Reports-Read     |
| HR employee records   | AP-HR-Employee-Records-Read | SG-HR-Employee-Records-Read |
| IT service desk tools | AP-IT-ServiceDesk-Tools     | SG-IT-ServiceDesk-Tools     |

Each access package is connected to a dedicated Microsoft Entra security group. Access is requested through entitlement management and assigned only after the configured approval workflow is completed.

## Request approval policies

| Access package              | Eligible requester | Approval required | Approver      | Justification required |
| --------------------------- | ------------------ | ----------------- | ------------- | ---------------------- |
| AP-Finance-Reports-Read     | Ava Finance        | Yes               | Riley Manager | Yes                    |
| AP-HR-Employee-Records-Read | Mia HR             | Yes               | Riley Manager | Yes                    |
| AP-IT-ServiceDesk-Tools     | Leo IT             | Yes               | Riley Manager | Yes                    |

Each access package uses a request approval policy to control who can request access and who must approve the request before access is assigned.

The policies are intentionally scoped to one requester per access package so each ticket workflow can be tested and documented clearly.

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
  01-repo-setup/
  02-entra-setup/
  03-access-packages/
  04-ticket-workflows/
  05-access-verification/
tickets/
README.md
```

## Evidence collected

Screenshots were collected throughout the lab to document the setup, request workflows, approval decisions, access assignments, and verification results.

Evidence includes:

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

Complete.

This lab includes configured Microsoft Entra security groups, fictional lab users, access packages, request approval policies, and three documented IAM ticket workflows.

The completed workflows demonstrate an approved Finance access request, a denied HR employee records request, and an approved IT service desk tools request with access assignment and group membership verification.

## Important note

This is a fictional lab environment created for portfolio and learning purposes. It does not include confidential, employer, customer, or production information.
