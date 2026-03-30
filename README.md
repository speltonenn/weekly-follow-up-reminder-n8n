# weekly-follow-up-reminder-n8n
Finds unanswered sent emails and delivers a single follow-up reminder every Monday.
# Weekly Email Follow-Up Reminder

A simple workflow that scans your Gmail sent folder every Monday and reminds you which emails are still waiting for a reply.

## How it works

1. Triggers every Monday at 10:00 AM
2. Fetches sent emails older than 5 days
3. Checks each thread for replies
4. Collects all unanswered emails
5. Sends you a single digest reminder

## Requirements

- n8n 
- Gmail account connected via OAuth2

## Setup

1. Import the workflow into n8n
2. Connect your Gmail account in the credentials
3. Adjust the schedule and email age filter if needed
4. Activate the workflow

## Notes

- The workflow does not send any emails on your behalf — it only notifies you
- Change `older_than:5d` in the Gmail search filter to adjust the time window
- The reminder digest is sent to your own Gmail address
