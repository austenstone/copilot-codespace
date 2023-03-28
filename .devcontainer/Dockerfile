ARG VARIANT=16
FROM mcr.microsoft.com/vscode/devcontainers/typescript-node:${VARIANT}

RUN npm install -g @githubnext/github-copilot-cli
RUN eval "$(github-copilot-cli alias -- "$0")"
RUN apt-get install -y java