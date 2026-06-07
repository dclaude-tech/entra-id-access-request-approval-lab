# TICKET-002: HR employee records read-only access

## Ticket summary

| Field | Details |
|---|---|
| Ticket ID | TICKET-002 |
| Requester | Mia HR |
| Requested access | AP-HR-Employee-Records-Read |
| Backing security group | SG-HR-Employee-Records-Read |
| Resource area | HR employee records |
| Access level | Read-only |
| Outcome | Denied |
| Ticket status | Closed |

## Request details

Mia HR requested read-only access to fictional HR employee records.

The requested access was tied to the AP-HR-Employee-Records-Read access package, which would assign membership to the SG-HR-Employee-Records-Read security group if approved.

## Business justification

Mia HR requested access to review employee information for department reporting.

## IAM review notes

The request required additional review because HR employee records may contain sensitive employee information.

The request did not include enough detail about the specific records, scope, or business need required to approve access to sensitive HR data. Based on least privilege, the request was denied.

## Approval decision

| Step | Reviewer | Decision | Notes |
|---|---|---|---|
| Stage 1 | Riley Manager | Denied | Request did not provide enough detail about the specific HR records, scope, or business need. |

## Access assignment status

Access was not assigned.

Because the request was denied, Mia HR did not receive a delivered access package assignment.

## Verification

After the denial, access was verified in two places:

- AP-HR-Employee-Records-Read showed no delivered assignment for Mia HR
- SG-HR-Employee-Records-Read showed no group membership for Mia HR

## Evidence

| Evidence | Screenshot |
|---|---|
| Request submitted | `screenshots/04-ticket-workflows/05-ticket-002-request-submitted.png` |
| Request denied | `screenshots/04-ticket-workflows/06-ticket-002-request-denied.png` |
| No access package assignment found | `screenshots/05-access-verification/07-ticket-002-no-assignment-found.png` |
| No security group membership found | `screenshots/05-access-verification/08-ticket-002-group-membership-not-found.png` |

## Closure notes

TICKET-002 was reviewed, denied, verified, and closed.

Mia HR did not receive HR employee records access because the request did not include enough detail to justify access to sensitive HR resources.
