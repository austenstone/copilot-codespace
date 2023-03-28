# ARG VARIANT=16
# FROM mcr.microsoft.com/vscode/devcontainers/typescript-node:${VARIANT}
FROM ubuntu:latest

RUN apt-get update

RUN apt install nodejs npm
RUN npm install -g @githubnext/github-copilot-cli
RUN echo 'eval "$(github-copilot-cli alias -- "$0")"' >> ~/.bashrc || echo 'Failed to setup alias convenience commands'
