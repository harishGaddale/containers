podman build -t redocly-cli-apline:v1.0.0 -f Containerfile .

podman run --name redocly-cli --rm -it -v $(pwd):/spec:Z redocly-cli-apline
