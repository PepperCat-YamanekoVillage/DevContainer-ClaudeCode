FROM mcr.microsoft.com/devcontainers/python:3.12

# Node.js (Claude Code用)
RUN curl -fsSL https://deb.nodesource.com/setup_22.x | bash - \
    && apt-get update \
    && apt-get install -y nodejs

# Claude Code
RUN npm install -g @anthropic-ai/claude-code

# 動作確認
RUN python --version \
    && node --version \
    && claude --version