# Documentation: Travel AssistantAgent

## Description
The "Travel AssistantAgent" workflow provides a chatbot-based travel assistant that integrates chat memory and AI-powered responses to assist users with travel-related queries.

## Nodes
1. **When chat message received**: Triggers the workflow upon receiving a chat message.
2. **MongoDB Chat Memory**: Stores chat history in MongoDB for context-aware responses.
3. **Google Gemini Chat Model**: Utilizes AI to generate responses based on user queries and stored chat context.

## Web Services Involved
- **MongoDB**: Used for storing chat memory.
- **Google Gemini AI**: Provides AI-powered chat responses.
