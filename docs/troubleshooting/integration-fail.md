---
layout: default
title: Integration Failures
parent: Troubleshooting
nav_order: 3
---

# Integration Failures

Issues when connecting third-party apps.

## 403 Forbidden

The connected user account does not have permission to perform the requested action.
**Fix:** Check the permissions of the user you authenticated with in the external app.

## Connection Refused

The external service might be down or blocking FlowPilot's IP addresses.
**Fix:** Whitelist FlowPilot's IP ranges in your firewall or security settings if you are connecting to an internal tool.

## Data Mapping Errors

"Field X is required but was empty."
**Fix:** Ensure that all required fields in an action step are mapped correctly from previous steps. data passed from a trigger might be null.
