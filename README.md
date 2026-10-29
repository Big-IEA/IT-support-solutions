
# Project: Helpdesk Admin Role Permission Test

## Goal
Show that least-privilege access works in Microsoft Entra ID: a Helpdesk
Administrator can reset passwords for standard users but not for admins.

## Environment
- Microsoft Entra ID lab tenant (free Azure account)
- Test users: SarahAdmin (Helpdesk Administrator), Mary (standard user)

## Steps
1. Created test users and a guest user
2. Assigned the Helpdesk Administrator role to SarahAdmin
3. Signed in as SarahAdmin in a private browser window
4. Reset Mary's password (standard user)
5. Tried to reset my Global Admin account's password

## Result
- Mary's password reset: Success (screenshot 1)
- Global Admin password reset: Blocked (screenshot 2)

## What I learned
- Helpdesk Administrator can only reset passwords for non-admin users
- Giving users only the access they need reduces security risk
- Role assignments should be tested, not assumed

## Skills shown
Entra ID, RBAC, least privilege, password reset, documentation
