---
layout: default
title: Common Errors
parent: Troubleshooting
nav_order: 1
---

# Common Errors

Here are some frequent error messages and how to resolve them.

## "Trigger Failed: Authentication Error"

This usually means the connection to your trigger app has expired or was revoked.
**Fix:** Go to **Apps** and re-authenticate the connection.

## "Rate Limit Exceeded"

You have hit the API rate limit for a connected service (e.g., sending too many Slack messages in a minute).
**Fix:** Add a **Delay** step in your workflow to space out actions.

## "AI Model Timeout"

The AI model took too long to generate a response. This can happen with complex prompts or very long input texts.
**Fix:** Try simplifying your prompt or splitting the input into smaller chunks.
