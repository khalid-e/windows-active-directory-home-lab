# Ticket 001 — User Unable to Sign In

## Issue

A user reported that they were unable to sign in to their domain account.

## Investigation

I checked the user's account in Active Directory Users and Computers (ADUC) and identified that the account had been disabled.

![Disabled domain user account in Active Directory](../screenshots/04-disabled-domain-account.png)

## Resolution

I opened the user's account properties and re-enabled the account by clearing the **Account is disabled** option.

![Active Directory account properties after re-enabling the user](../screenshots/05-enabled-domain-account.png)

## Verification

Confirmed in Active Directory that the user account was enabled and available for authentication.
