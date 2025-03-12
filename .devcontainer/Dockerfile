FROM amazonlinux:2

# Install necessary packages
RUN yum update -y && \
    yum install -y python3 python3-pip zip && \
    yum clean all

# Ensure the vscode user exists and set permissions
RUN useradd -m -s /bin/bash vscode && \
    mkdir -p /home/vscode && \
    chown -R vscode:vscode /home/vscode

USER vscode
WORKDIR /home/vscode
