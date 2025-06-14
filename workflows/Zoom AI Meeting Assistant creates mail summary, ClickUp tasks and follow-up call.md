# Zoom AI Meeting Assistant

## Description
This workflow uses AI to summarize Zoom meeting recordings, create tasks in ClickUp, and schedule follow-up calls.

## Nodes
1. **OpenAI Chat Model**: Processes meeting transcripts using OpenAI's GPT-4 model.
2. **Manual Trigger**: Initiates the workflow manually.
3. **No Recording/Transcript available**: Stops the workflow if no recording or transcript is available.

## Web Services Involved
- **Zoom**: Source of meeting recordings.
- **OpenAI API**: Used for transcript summarization.
- **ClickUp**: Used for task creation.
