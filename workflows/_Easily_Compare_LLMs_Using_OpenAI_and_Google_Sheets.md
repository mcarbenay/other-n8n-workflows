# Easily Compare LLMs Using OpenAI and Google Sheets

## Description
This workflow allows users to evaluate and compare the outputs of two language models (LLMs) before choosing one for production. It logs responses into a Google Sheet for manual or automated evaluation.

## Nodes
1. **When chat message received**: Triggers the workflow upon receiving a chat message.
2. **Loop Over Items**: Iterates over items for batch processing.
3. **Simple Memory**: Manages memory context for chat sessions.
4. **Chat Memory Manager**: Handles retrieval of prior context for qualitative evaluation.
5. **OpenRouter Chat Model**: Processes user input using OpenRouter models.
6. **AI Agent**: Dynamically selects models for evaluation.
7. **Concatenate Chat Answers**: Combines model responses for display.
8. **Group Model Outputs for Evaluation**: Aggregates model outputs for Google Sheets.
9. **Add Model Results to Google Sheet**: Logs responses and evaluations into a Google Sheet.
10. **Prepare Data for Chat and Google Sheets**: Prepares data for logging and chat display.
11. **Define Models to Compare**: Specifies the models to be compared.
12. **Split Models into Items**: Splits model IDs for processing.
13. **Set model, sessionId, chatInput, sessionIdBase**: Prepares variables for model evaluation.
14. **Set Output for Chat UI**: Formats output for chat display.

## Web Services
- **Google Sheets**: Logs model responses and evaluations.
- **OpenRouter API**: Processes user input using specified LLMs.

## Summary
This workflow simplifies the comparison of LLMs by integrating chat interfaces and Google Sheets for structured evaluation.
