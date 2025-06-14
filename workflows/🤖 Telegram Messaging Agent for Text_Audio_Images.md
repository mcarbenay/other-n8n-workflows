# Telegram Messaging Agent for Text/Audio/Images

## Description
This workflow processes Telegram messages, including text, audio, and images, and provides error handling for unsupported formats.

## Nodes
1. **Check User & Chat ID**: Validates the user and chat ID from incoming Telegram messages.
2. **Error message**: Sends an error message to the user if the message cannot be processed.
3. **Sticky Note**: Provides a visual note for workflow documentation.

## Web Services Involved
- **Telegram**: Used for messaging and error handling.
