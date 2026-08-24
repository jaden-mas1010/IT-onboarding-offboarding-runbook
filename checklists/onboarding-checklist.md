# New Hire Onboarding Checklist

Target: complete all steps before employee's first-day 9:00 AM start. SLA: initiate within 3 business days of hire confirmation from People team.

## 1. Pre-arrival (2-3 days before start date)

- [ ] Confirm role, department, and manager from People team ticket
- [ ] Determine device type required (Windows or macOS) based on role
- [ ] Create M365 account (Exchange Online mailbox, license assignment)
- [ ] Add user to relevant M365 security groups and distribution lists
- [ ] Set up conditional access / MFA enrollment link to send on day one
- [ ] Provision device from asset inventory, update asset tracker with assignment
- [ ] Image/reset device to standard build

## 2. Windows device setup

- [ ] Join device to Azure AD / Intune enrollment
- [ ] Confirm BitLocker encryption enabled
- [ ] Install core application stack (M365 Apps, Teams, VPN client, endpoint protection)
- [ ] Apply baseline security policies (screen lock timeout, password policy)
- [ ] Verify Windows Update is current
- [ ] Test login with new user credentials before handoff

## 3. macOS device setup

*(Documented to Apple Business Manager standard — see README scope note)*

- [ ] Enroll device in Apple Business Manager / MDM (e.g., Jamf or Intune for Mac)
- [ ] Confirm FileVault disk encryption enabled and recovery key escrowed
- [ ] Push core application stack via MDM (M365 Apps, Teams, VPN client, endpoint protection)
- [ ] Configure Gatekeeper and firewall baseline settings
- [ ] Enroll in automatic macOS security updates
- [ ] Verify device check-in with MDM before handoff

## 4. Account and access provisioning

- [ ] Assign M365 license (matched to role requirements)
- [ ] Add to Teams channels relevant to department
- [ ] Grant access to shared drives / SharePoint sites per role
- [ ] Provision any role-specific SaaS tool access (ticketed separately if outside standard stack)
- [ ] Set temporary password with forced reset on first login
- [ ] Enroll user in MFA

## 5. Day one

- [ ] Hand off device (or ship with setup guide if remote)
- [ ] Walk new hire through login, MFA enrollment, and password reset
- [ ] Confirm access to email, Teams, and core shared resources
- [ ] Log completion in ticketing system with timestamp
- [ ] Update asset tracker: device status = "assigned," owner = new hire

## 6. Close-out

- [ ] Confirm with new hire (or manager) that all access is working
- [ ] Close onboarding ticket with resolution notes
- [ ] File any KB article gaps discovered during the process
