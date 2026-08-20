podman build -t redocly-cli-apline:v1.0.0 -f Containefile .

podman run --name redocly-cli --rm -it -v $(pwd):/spec:Z localhost/redocly-cli-apline
