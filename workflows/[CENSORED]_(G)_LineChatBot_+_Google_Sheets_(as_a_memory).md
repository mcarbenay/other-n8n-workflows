# (G) LineChatBot + Google Sheets (as a memory)

## Description
This workflow integrates a Line chatbot with Google Sheets to store and retrieve chat history. It uses AI to provide context-aware responses based on previous interactions.

## Nodes
1. **Webhook**: Receives incoming messages from the Line API.
2. **Edit Fields**: Extracts relevant fields from the incoming message.
3. **Get History**: Retrieves chat history from Google Sheets.
4. **Prepare Prompt**: Constructs a prompt for the AI agent using the retrieved history.
5. **AI Agent**: Generates context-aware responses using the Google Gemini Chat Model.
6. **Split History**: Splits chat history into manageable chunks for storage.
7. **Save History**: Updates Google Sheets with the latest chat history.
8. **HTTP Request**: Sends the AI-generated response back to the Line API.

## Web Services
- **Line API**: Handles incoming and outgoing messages.
- **Google Sheets**: Stores and retrieves chat history.
- **Google Gemini Chat Model**: Provides AI-driven responses.

## Summary
This workflow enables a Line chatbot to maintain context across conversations by leveraging Google Sheets for memory and Google Gemini for AI responses.
