# Cloud Chatbot Development Lab

A Jupyter-based hands-on lab for building a simple cloud-hosted chatbot with the Anthropic Python SDK. The lab lives in one notebook, `ClaudeChatbotDevelopment.ipynb`, and covers five parts: API setup, conversation design and personas, memory management, safety guardrails, and LLM metrics.

## Prerequisites

- Python 3.9 or later
- An Anthropic API key
- Optional: a base URL, if your organization uses a custom API endpoint

## Step 1: Install the tools

```bash
pip install anthropic jupyter
```

## Step 2: Get the notebook

Clone this repository, or download `ClaudeChatbotDevelopment.ipynb` directly.

```bash
git clone https://github.com/Tech-hub-bytes/cloud-chatbot-development-lab.git
cd cloud-chatbot-development-lab
```

## Step 3: Add your credentials

The notebook contains two placeholders in the API setup cell. Never commit real keys.

- `<YOUR_API_KEY>`: replace with your Anthropic API key. For a safer setup, export it as an environment variable (`ANTHROPIC_API_KEY`) and remove the hardcoded line.
- `<YOUR_BASE_URL>`: replace with your API endpoint, or delete the `base_url` argument to use the default endpoint.

## Step 4: Start Jupyter

```bash
jupyter notebook ClaudeChatbotDevelopment.ipynb
```

Your browser opens the notebook.

## Step 5: Run the notebook in order

1. **Import and API setup.** Remove the `import chatbot` line if you are running outside the original lab environment. Then run the setup cell and a first request to confirm the connection.
2. **Conversation design and personas.** Compare single-turn and multi-turn chats, then run the chat loop. Type `quit` to exit.
3. **Memory management.** Save and restore a session to `demo_session.json`, and summarize conversation history into facts.
4. **Safety guardrails.** Test a scoped system prompt against a risky request.
5. **LLM metrics.** Measure request latency and track input and output tokens.

Run each cell from top to bottom. Restart the kernel if you change the API key or base URL.

## Troubleshooting

- **Authentication error:** check that your API key is correct and active.
- **Connection error:** check the base URL, or remove the `base_url` argument to use the default endpoint.
- **`ModuleNotFoundError: chatbot`:** remove the `import chatbot` line, which only works inside the original lab environment.

## Video and channel

- Video: [Cloud Chatbot Development: Hands-On Lab Walkthrough](https://youtu.be/kMHJgykcJPo), which shows this lab step by step.
- Channel: [DataMind AI on YouTube](https://www.youtube.com/@DataMindAI-i6d)
