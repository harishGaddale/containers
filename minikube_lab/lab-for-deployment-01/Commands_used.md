podman search docker.io/nginx:mainline-alpine3.23-slim

kubectl create deployment harishnginx --image=docker.io/library/nginx:latest --replicas=2 --dry-run=client -o yaml > harishnginx_config.yaml