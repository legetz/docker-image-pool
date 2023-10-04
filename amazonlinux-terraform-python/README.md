# Build image
- `docker build --platform linux/amd64 -t jokinlex/amazonlinux-terraform-python:terraform-1.5.7-python-3.11 .`

# Start image locally
```
docker rm amazonlinux-terraform-python
docker create --name amazonlinux-terraform-python -i -t jokinlex/amazonlinux-terraform-python:terraform-1.5.7-python-3.11
docker container start --attach -i amazonlinux-terraform-python
```