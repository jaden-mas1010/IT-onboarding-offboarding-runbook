# Employee Offboarding Checklist

Target: all access revoked by end of employee's last working day. SLA: initiate immediately on receipt of offboarding notice from People team; complete within 4 hours for same-day departures, or by end of last day for planned departures.

## 1. Pre-departure prep (on notice)

- [ ] Confirm last working day and departure type (voluntary, involuntary, planned, immediate) from People team ticket
- [ ] Flag immediate/involuntary departures for expedited same-hour processing
- [ ] Identify all systems and accounts tied to the employee (M365, SaaS tools, shared drives, VPN)
- [ ] Notify manager of any data handoff needed before access is revoked

## 2. Account deprovisioning

- [ ] Disable M365 account sign-in (block, do not delete immediately)
- [ ] Revoke all active sessions and refresh tokens
- [ ] Remove MFA methods
- [ ] Convert mailbox to shared/archived mailbox if retention required
- [ ] Set up mail forwarding/auto-reply if agreed with manager
- [ ] Remove from all M365 security groups and distribution lists
- [ ] Revoke access to shared drives, SharePoint sites, Teams channels
- [ ] Deprovision any role-specific SaaS tool accounts

## 3. Device reclaim — Windows

- [ ] Remotely lock device via Intune if remote employee
- [ ] Schedule device return (courier for remote, in-person for office-based)
- [ ] On return: verify device physically, check for damage
- [ ] Wipe device to standard build (full reset, not just account removal)
- [ ] Confirm BitLocker key rotation logged
- [ ] Update asset tracker: status = "returned/wiped," available for reissue

## 4. Device reclaim — macOS

*(Documented to Apple Business Manager standard — see README scope note)*

- [ ] Remotely lock device via MDM if remote employee
- [ ] Schedule device return
- [ ] On return: verify device physically, check for damage
- [ ] Remotely wipe via MDM (Erase All Content and Settings) or full reinstall
- [ ] Remove from Apple Business Manager device assignment
- [ ] Update asset tracker: status = "returned/wiped," available for reissue

## 5. Security and compliance

- [ ] Confirm no active sessions remain across all systems (audit log check)
- [ ] Remove employee from any privileged access groups (admin, finance systems, etc.) as priority-one step
- [ ] Document offboarding completion with timestamps for compliance audit trail
- [ ] Flag any anomalies (e.g., recent large file downloads) to security lead per policy

## 6. Close-out

- [ ] Confirm all checklist items complete with manager/People team
- [ ] Close offboarding ticket with full resolution notes and timestamps
- [ ] Reassign or archive licenses freed up by offboarding
