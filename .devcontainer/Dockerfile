ARG IMAGE
ARG RELEASE
# Use Ubuntu 24.04 as the base image
FROM rightclickscript/devcontainers:${IMAGE}-${RELEASE}

RUN rm /bin/sh && ln -s /bin/bash /bin/sh

# Switch to the non-root user
ARG USERNAME=vscode
USER $USERNAME

# Set the default user to vscode
WORKDIR /home/vscode/