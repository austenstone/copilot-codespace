ARG VARIANT=16
FROM mcr.microsoft.com/vscode/devcontainers/typescript-node:${VARIANT}

RUN sudo apt-get update

RUN npm install -g @githubnext/github-copilot-cli
RUN echo 'eval "$(github-copilot-cli alias -- "$0")"' >> ~/.zshrc || echo 'eval "$(github-copilot-cli alias -- "$0")"' >> ~/.bashrc || echo 'Failed to setup alias convenience commands'
