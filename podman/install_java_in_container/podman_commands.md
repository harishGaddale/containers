podman run -ti registry.access.redhat.com/ubi8/ubi bash

# install openjdk21 
yum install java-21-openjdk-devel

# Stop the container that is running
podman stop

# Commit changes with new name

podman commit unruffled_hofstadter harishubi8jdk21