FROM amazonlinux:2

# Install necessary packages
RUN yum update -y && \
    yum install -y python3 python3-pip zip && \
    yum clean all

# Install Docker (optional, for consistency)
RUN yum install -y docker && \
    usermod -aG docker vscode && \
    systemctl enable docker && systemctl start docker

# Ensure the vscode user can run commands
USER vscode
WORKDIR /home/vscode