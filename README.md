# IAM Access Request and Approval Lab | Microsoft Entra ID

## Overview

This project is a hands-on IAM access request and approval lab built in Microsoft Entra ID.

I used this lab to practice the access request process from intake to closure: reviewing the request, checking the business justification, routing it for approval, verifying the assignment, and documenting the ticket outcome.

## Scenario

Northstar Identity Lab is a fictional organization with department-based access needs across Finance, HR, and IT.

In this lab, users request access to specific resources through Microsoft Entra entitlement management. Each request is reviewed based on business need, least privilege, approval requirements, and verification evidence.

## Workflow demonstrated

This lab demonstrates an IAM access request workflow, including:

* Creating Microsoft Entra users, groups, and access packages
* Configuring request and approval policies
* Submitting access requests as fictional users
* Approving or denying requests based on business context
* Verifying access package assignments and group membership
* Documenting ticket outcomes

## Lab environment

The lab uses a Microsoft Entra ID tenant named **Northstar Identity Lab**.

All users, groups, access packages, and tickets were created only for learning and portfolio documentation.

## Lab identities

| User          | Role in lab             | Workflow use                              |
| ------------- | ----------------------- | ----------------------------------------- |
| Ava Finance   | Finance requester       | Requests Finance reports read-only access |
| Mia HR        | HR requester            | Requests HR employee records access       |
| Leo IT        | IT requester            | Requests IT service desk tools access     |
| Riley Manager | Approver/resource owner | Reviews access requests                   |

The lab identities are fictional users created for access request and approval testing.

## Ticket workflows

| Ticket     | Access request                       | Outcome               |
| ---------- | ------------------------------------ | --------------------- |
| TICKET-001 | Finance reports read-only access     | Approved              |
| TICKET-002 | HR employee records read-only access | Denied                |
| TICKET-003 | IT service desk tools access         | Approved after review |

The denied HR request was included to show that IAM review is not only about granting access. Some requests should be rejected when the business justification does not support the level of access requested.

## Ticket documentation

| Ticket     | Documentation                                                                         | Summary                                       |
| ---------- | ------------------------------------------------------------------------------------- | --------------------------------------------- |
| TICKET-001 | [TICKET-001 finance reports read](tickets/TICKET-001-finance-reports-read.md)         | Approved Finance reports access request       |
| TICKET-002 | [TICKET-002 HR employee records read](tickets/TICKET-002-hr-employee-records-read.md) | Denied HR employee records access request     |
| TICKET-003 | [TICKET-003 IT service desk tools](tickets/TICKET-003-it-servicedesk-tools.md)        | Approved IT service desk tools access request |

Each ticket documents the requester, requested access, business justification, IAM review notes, approval decision, verification results, evidence, and closure notes.

## Access model

| Resource area         | Access package              | Backing security group      |
| --------------------- | --------------------------- | --------------------------- |
| Finance reports       | AP-Finance-Reports-Read     | SG-Finance-Reports-Read     |
| HR employee records   | AP-HR-Employee-Records-Read | SG-HR-Employee-Records-Read |
| IT service desk tools | AP-IT-ServiceDesk-Tools     | SG-IT-ServiceDesk-Tools     |

Each access package is connected to a dedicated Microsoft Entra security group.

Access is requested through entitlement management and assigned only after the configured approval workflow is completed.

## Request approval policies

| Access package              | Eligible requester | Approval required | Approver      | Justification required |
| --------------------------- | ------------------ | ----------------- | ------------- | ---------------------- |
| AP-Finance-Reports-Read     | Ava Finance        | Yes               | Riley Manager | Yes                    |
| AP-HR-Employee-Records-Read | Mia HR             | Yes               | Riley Manager | Yes                    |
| AP-IT-ServiceDesk-Tools     | Leo IT             | Yes               | Riley Manager | Yes                    |

Each access package uses a request approval policy to control who can request access and who must approve the request before access is assigned.

## IAM analyst skills practiced

* Access request review
* Business justification review
* Least-privilege decision making
* Approval and denial documentation
* Microsoft Entra entitlement management
* Access verification
* Ticket-style documentation

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

Screenshots were collected throughout the lab to document setup, request workflows, approval decisions, access assignments, and verification results.

Evidence includes Microsoft Entra users, groups, access packages, approval policies, submitted requests, approval and denial decisions, assignment verification, and closed ticket documentation.

## Project takeaways

This lab helped reinforce that access approval depends on more than whether a user asks for access. The request needs to match the user’s role, the business justification needs to be clear, and the final access assignment needs to be verified.

The most useful part of this lab was documenting different outcomes. One request was approved, one was denied, and one was approved after review. That made the workflow closer to real IAM support work.

## Project status

Complete.

This lab includes Microsoft Entra security groups, fictional lab users, access packages, request approval policies, three simulated IAM ticket workflows, and access verification evidence.

## Scope notes

This lab uses fictional users, access packages, security groups, and simulated tickets created for portfolio documentation.

The ticket files are written in Markdown to represent IAM ticket documentation. This lab does not use ServiceNow, Jira, production data, customer data, or real business applications.

The access package policies were intentionally scoped to one requester per package so each workflow could be tested and documented clearly.
