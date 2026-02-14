README.md (copy–paste exactly)
# Basic Dockerfile – Hello Captain

This project demonstrates the most basic usage of Docker by creating a Docker image that prints a message to the console and exits.

Project reference:
https://roadmap.sh/projects/basic-dockerfile

---

## Project Objective

The goal of this project is to understand:

- How a Dockerfile works
- How to build a Docker image
- How to run a container that performs a single task
- How Docker images behave when the container exits

This project intentionally keeps things minimal to focus on core Docker concepts.

---

## Dockerfile Explanation

- Uses `alpine:latest` as the base image
- Executes a single command
- Prints `Hello, Captain!` to the console
- Exits immediately after execution

---

## Dockerfile

```Dockerfile
FROM alpine:latest
CMD ["echo", "Hello, Captain!"]
How to Build the Image

Run this command from the project root:

docker build -t hello-captain .
How to Run the Container
docker run --rm hello-captain

Expected output:

Hello, Captain!

The container stops automatically after printing the message. This is expected behavior.

Optional Enhancement

The project can be extended to accept a name as an argument and print:

Hello, <name>!

This enhancement is optional and not required for the base project.

Skills Demonstrated

Docker installation and usage

Writing minimal Dockerfiles

Building Docker images

Running containers on Linux / cloud VMs


---

## `.gitignore` file (recommended)

Create a `.gitignore` file even if it’s small. It shows discipline.

```gitignore
*.log
*.tmp
.DS_Store# basic-docker-file
