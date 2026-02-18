---
layout: default
title: Task Pipelines
parent: Features
nav_order: 2
---

# Task Pipelines

Pipelines allow you to chain multiple workflows together or process large datasets in parallel.

## Sequential vs. Parallel Execution

### Sequential Pipelines
Execute steps one after another. If one step fails, the entire pipeline halts (unless error handling is configured). Best for dependent tasks.

### Parallel Processing
Split a large list of items (e.g., a CSV of 10,000 leads) into chunks and process them simultaneously. This significantly reduces total execution time.

## Error Handling

Pipelines come with built-in error handling logic:
- **Retry:** Automatically retry a failed step up to 3 times with exponential backoff.
- **Ignore:** Log the error and continue to the next step.
- **Fallback:** execute an alternative path if the primary action fails.
