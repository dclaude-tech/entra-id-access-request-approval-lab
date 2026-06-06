# TICKET-002: HR employee records read-only access

## Ticket summary

| Field                  | Details                     |
| ---------------------- | --------------------------- |
| Ticket ID              | TICKET-002                  |
| Requester              | Mia HR                      |
| Requested access       | AP-HR-Employee-Records-Read |
| Backing security group | SG-HR-Employee-Records-Read |
| Resource area          | HR employee records         |
| Access level           | Read-only                   |
| Planned outcome        | Denied                      |
| Ticket status          | Open                        |

## Request details

Mia HR is requesting read-only access to fictional HR employee records.

The requested access is tied to the AP-HR-Employee-Records-Read access package, which would assign membership to the SG-HR-Employee-Records-Read security group if approved.

## Business justification

Mia HR is requesting access to review employee information for department reporting.

## IAM review notes

This request requires additional scrutiny because HR employee records may contain sensitive employee information.

Before access can be granted, the request should clearly explain the business need, scope, and reason the requester needs access to this specific HR resource.

## Approval plan

| Step    | Reviewer      | Planned action                                                                                           |
| ------- | ------------- | -------------------------------------------------------------------------------------------------------- |
| Stage 1 | Riley Manager | Review the request and deny if the business justification is not specific enough for sensitive HR access |

## Access assignment status

Access has not been assigned.

## Verification plan

After the decision, verify that:

* No delivered access package assignment exists if the request is denied
* Mia HR is not added to SG-HR-Employee-Records-Read if the request is denied
* The ticket is updated with evidence and closure notes

## Evidence

Evidence will be added after the request is submitted, reviewed, denied, and verified.
