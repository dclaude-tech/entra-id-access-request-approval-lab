# TICKET-001: Finance reports read-only access

## Ticket summary

| Field                  | Details                 |
| ---------------------- | ----------------------- |
| Ticket ID              | TICKET-001              |
| Requester              | Ava Finance             |
| Requested access       | AP-Finance-Reports-Read |
| Backing security group | SG-Finance-Reports-Read |
| Resource area          | Finance reports         |
| Access level           | Read-only               |
| Outcome                | Approved                |
| Ticket status          | Closed                  |

## Request details

Ava Finance requested read-only access to fictional Finance reporting resources.

The requested access is tied to the AP-Finance-Reports-Read access package, which assigns membership to the SG-Finance-Reports-Read security group after approval.

## Business justification

Ava Finance requested read-only access to Finance reporting resources to review department reporting data.

## IAM review notes

The request aligned with the requester’s fictional Finance role.

The requested access was limited to read-only Finance reporting access, which supports least privilege because it does not grant broad administrative access or unrelated department access.

## Approval decision

| Step    | Reviewer      | Decision | Notes                                                                          |
| ------- | ------------- | -------- | ------------------------------------------------------------------------------ |
| Stage 1 | Riley Manager | Approved | Request aligned with the requester’s fictional Finance role and business need. |

## Access assignment status

Access was assigned through the AP-Finance-Reports-Read access package after approval.

The access package assignment was delivered to Ava Finance.

## Verification

After approval, access was verified in two places:

* AP-Finance-Reports-Read showed Ava Finance with a delivered assignment
* SG-Finance-Reports-Read showed Ava Finance as a direct group member

## Evidence

| Evidence                            | Screenshot                                                                       |
| ----------------------------------- | -------------------------------------------------------------------------------- |
| Request submitted                   | `screenshots/04-ticket-workflows/01-ticket-001-request-submitted.png`            |
| Request approved                    | `screenshots/04-ticket-workflows/02-ticket-001-request-approved.png`             |
| Access package assignment delivered | `screenshots/05-access-verification/03-ticket-001-assignment-delivered.png`      |
| Security group membership verified  | `screenshots/05-access-verification/04-ticket-001-group-membership-verified.png` |

## Closure notes

TICKET-001 was approved, assigned, verified, and closed.

Ava Finance received read-only Finance reports access through the documented access request and approval workflow.
