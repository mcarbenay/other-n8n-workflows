# Documentation: Log errors and avoid sending too many emails

## Description
The "Log errors and avoid sending too many emails" workflow logs errors into a database and prevents excessive email notifications.

## Nodes
1. **Error Trigger**: Captures errors during workflow execution.
2. **Insert Log**: Logs error details into a PostgreSQL database.

## Web Services Involved
- **PostgreSQL**: Used for storing error logs.
