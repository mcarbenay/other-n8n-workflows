# Chat with local LLMs using n8n and Ollama

## Description
This n8n workflow allows you to seamlessly interact with your self-hosted Large Language Models (LLMs) through a user-friendly chat interface. By connecting to Ollama, a powerful tool for managing local LLMs, you can send prompts and receive AI-generated responses directly within n8n.

## Nodes Used
1. **When chat message received**: Captures the user's input from the chat interface.
2. **Chat LLM Chain**: Sends the input to the Ollama server and receives the AI-generated response.
3. **Ollama Chat Model**: Connects to the local Ollama server.
4. **Sticky Note**: Provides setup instructions and workflow details.

## Services Used
- **Ollama**: A tool for managing local LLMs.

## Setup Steps
- Ensure Ollama is installed and running on your machine before executing this workflow.
- Edit the Ollama address if different from the default.
- If running in Docker, make sure that the n8n container has access to the host's network in order to connect to Ollama. You can do this by passing `--net=host` option when starting the n8n Docker container.
