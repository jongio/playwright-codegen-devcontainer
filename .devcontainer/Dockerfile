FROM mcr.microsoft.com/vscode/devcontainers/universal:1-focal
USER root
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && npm i -D @playwright/test
USER codespace
RUN npx -q playwright install \
     && npx playwright install-deps