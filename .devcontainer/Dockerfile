FROM mcr.microsoft.com/vscode/devcontainers/go:dev-1.23-bookworm

# This will be set to true when running in VSCode
ARG INTERACTIVE="false"
ARG USERNAME=vscode
ARG USER_UID=1000
ARG USER_GID=$USER_UID

RUN apt-get update && apt-get install -y curl gnupg lsb-release bash-completion --no-install-recommends \
    && apt-get clean -y && rm -rf /var/lib/apt/lists/*
    
USER $USERNAME