ARG VARIANT=16
FROM mcr.microsoft.com/vscode/devcontainers/typescript-node:${VARIANT}

RUN apt-get update -y 

RUN npm install -g @githubnext/github-copilot-cli

RUN echo 'eval "$(github-copilot-cli alias -- "$0")"' >> /home/node/.bashrc || echo 'Failed to setup alias convenience commands'
