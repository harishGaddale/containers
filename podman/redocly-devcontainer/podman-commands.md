# pull the image
podman pull ghcr.io/redocly/cli
# lint: check for errors and warnings in the OpenAPI specification
podman run --rm -v $PWD:/spec redocly/cli lint openapi.yaml
# bundle: convert the OpenAPI specification to JSON format
podman run --rm -v $PWD:/spec redocly/cli bundle updated-api.yaml --output updated-api.json