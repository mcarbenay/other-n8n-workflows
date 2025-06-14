# Documentation: v1 helper - Find params with affected expressions

## Description
The "v1 helper - Find params with affected expressions" workflow identifies parameters in active workflows that contain specific expressions affected by predefined extensions.

## Nodes
1. **Manual Trigger**: Allows manual initiation of the workflow.
2. **n8n**: Fetches active workflows for analysis.
3. **Find params with affected expressions**: Executes JavaScript code to locate parameters with affected expressions.

## Web Services Involved
- **n8n API**: Used to retrieve active workflows.
