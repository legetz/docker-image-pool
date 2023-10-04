FROM public.ecr.aws/lambda/python:3.11

# 2023-10-04:
# - Python 3.11.5
# - Terraform v1.5.7

# Upgrade pip
RUN pip install --upgrade pip

# Install Terraform
RUN yum install -y yum-utils shadow-utils
RUN yum-config-manager --add-repo https://rpm.releases.hashicorp.com/AmazonLinux/hashicorp.repo
RUN yum -y install terraform

ENTRYPOINT ["/bin/bash"]