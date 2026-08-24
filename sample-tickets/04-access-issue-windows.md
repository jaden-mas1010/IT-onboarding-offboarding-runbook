# Ticket #IT-1004 — Unable to Access Shared Drive (Windows)

**Requested by:** End user (Finance department)
**Assigned to:** J. Mascarenhas
**Priority:** Medium
**SLA target:** 4 business hours (standard access issue)
**Status:** Resolved

## Summary
User reports "Access Denied" error when attempting to open the Finance shared drive on their Windows laptop. Reports it worked yesterday.

## Timeline

| Timestamp | Action |
|---|---|
| 2026-08-20 10:05 | Ticket received, user contacted to confirm exact error and steps to reproduce |
| 2026-08-20 10:12 | User confirmed error message and provided screenshot |
| 2026-08-20 10:15 | Checked user's group membership in Azure AD — confirmed still in Finance security group |
| 2026-08-20 10:20 | Checked SharePoint site permissions — found user had been inadvertently removed during a recent group cleanup |
| 2026-08-20 10:30 | Re-added user to correct SharePoint permission group |
| 2026-08-20 10:35 | Asked user to sign out and back in to refresh token, confirmed access restored |
| 2026-08-20 10:40 | Root cause noted: recent bulk permission cleanup script did not account for this user's dual-department role |
| 2026-08-20 10:45 | Ticket resolved, flagged root cause for review to prevent recurrence |

**Resolution time:** 40 minutes (against 4 business hour SLA)

## Resolution notes
Access restored same day, well within SLA. Root cause traced to a permissions cleanup gap rather than a device issue — flagged to prevent similar tickets for other dual-role employees. Added a note to the KB article on shared drive access troubleshooting.
