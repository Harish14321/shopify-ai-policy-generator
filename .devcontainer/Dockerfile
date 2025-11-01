# Use official devcontainer base image
FROM mcr.microsoft.com/devcontainers/javascript-node:20

# Install shopify CLI dependencies and ngrok if needed
USER root
RUN apt-get update && apt-get install -y curl ca-certificates gnupg2 && rm -rf /var/lib/apt/lists/*

# Set non-root user back
USER node

# Ensure workspace folder exists
WORKDIR /workspaces/shopify-ai-policy-generator

# Default exposed port
EXPOSE 8081

# Default command (will be overridden by Codespaces)
CMD ["sleep", "infinity"]
