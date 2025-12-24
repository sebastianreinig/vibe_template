# Frontend Development Container
# Customize this Dockerfile based on your tech stack

FROM node:20-bookworm

# Install additional tools
RUN apt-get update && apt-get install -y \
    git \
    curl \
    && rm -rf /var/lib/apt/lists/*

# Set working directory
WORKDIR /workspace

# Default command
CMD ["bash"]
