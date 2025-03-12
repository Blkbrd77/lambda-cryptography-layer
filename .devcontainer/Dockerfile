FROM amazonlinux:2

# Install necessary packages
RUN yum update -y && \
    yum install -y python3 python3-pip zip && \
    yum clean all

# Set working directory
WORKDIR /home/vscode

# Use the default Codespaces user (vscode)
USER vscode
