# 🤖 Calendar Agent

## Description
The Calendar Agent workflow manages calendar-related tasks using OpenAI's GPT-4 model for processing and error handling. It supports creating, updating, deleting, and fetching events in a user's calendar.

## Nodes
1. **OpenAI Chat Model**: Utilizes GPT-4 for AI-driven calendar management.
2. **Try Again**: Handles errors and retries tasks.
3. **Success**: Confirms successful operations.
4. **Calendar Agent**: Acts as the main AI agent for calendar-related tasks.
5. **Create Event with Attendee**: Creates events with participants.
6. **Create Event**: Creates solo events.
7. **Get Events**: Fetches calendar schedules.
8. **Delete Event**: Deletes specified events.
9. **Update Event**: Updates event details.
10. **When Executed by Another Workflow**: Triggers execution from other workflows.

## Web Services
- **Google Calendar**: Used for event creation, deletion, and updates.
- **OpenAI GPT-4**: Provides AI-driven decision-making and task execution.

## Summary
This workflow simplifies calendar management by integrating AI capabilities with Google Calendar tools.
