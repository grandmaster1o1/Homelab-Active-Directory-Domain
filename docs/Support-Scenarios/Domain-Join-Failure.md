# HD-003 Domain Join Failure

## Issue

Workstation unable to join domain.

## Error

"The specified domain either does not exist or could not be contacted."

## Investigation

Checked:

- Network connectivity
- IP configuration
- DNS server settings

Commands:

ipconfig /all

ping DC01

nslookup homelab.local

## Root Cause

Client configured with incorrect DNS server.

## Resolution

Changed DNS server to Domain Controller IP.

## Verification

Successfully joined workstation to domain.
