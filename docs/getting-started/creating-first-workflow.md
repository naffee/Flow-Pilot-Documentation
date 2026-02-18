---
layout: default
title: Creating Your First Workflow
parent: Getting Started
nav_order: 2
---

# Creating Your First Workflow

In this guide, we will walk you through creating a simple workflow that monitors a Gmail inbox for urgent emails and sends a summary to Slack.

## Step 1: Create a New Workflow

1. Log in to your FlowPilot Dashboard.
2. Click the **+ New Workflow** button in the top right corner.
3. Name your workflow: `Urgent Email Summarizer`.

## Step 2: Set Up the Trigger

1. Click on the **Add Trigger** node.
2. Search for **Gmail** and select **New Email Matching Search**.
3. Connect your Google account.
4. In the search query field, enter: `label:urgent`.
5. Click **Save & Test** to verify the connection.

## Step 3: Add an AI Analysis Step

Now, let's use FlowPilot's AI engine to summarize the email content.

1. Click the **+** button after the trigger node.
2. Select **FlowPilot AI** from the app list.
3. Choose the **Summarize Text** action.
4. In the **Input Text** field, map the `Body Plain` data from the Gmail trigger.
5. Set the summary length to `Brief`.

## Step 4: Send Notification to Slack

1. Add another step by clicking **+**.
2. Select **Slack** and choose **Send Channel Message**.
3. Connect your Slack account and select the `#urgent-alerts` channel.
4. In the **Message Text** field, enter:
   ```text
   🚨 *Urgent Email Received*
   From: {{Gmail.From}}
   Subject: {{Gmail.Subject}}

   *Summary:*
   {{FlowPilotAI.Summary}}
   ```
5. Click **Save**.

## Step 5: Activate

Toggle the **Active** switch in the top toolbar to turn on your workflow. Congratulations! You have just deployed your first AI-powered automation.
