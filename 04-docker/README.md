# Lab 04 — Docker Containerization

## Objective

Install and configure Docker on the macOS host and use containerized applications as part of the cybersecurity laboratory.

## Environment

- Host: MacBook Pro 2019
- Processor: Intel Core i5
- RAM: 8 GB
- Operating System: macOS
- Container Platform: Docker Desktop

## Why Docker?

Docker provides a convenient way to package and run applications in isolated containers.

For a cybersecurity laboratory, containers are useful because intentionally vulnerable applications can be deployed, tested, stopped, removed, and recreated without installing their dependencies directly on the host operating system.

## Docker Concepts

### Image

A Docker image is a read-only template used to create containers.

### Container

A container is a running instance of a Docker image.

### Port Mapping

Docker can expose a container's service through a port on the host.

For example:

```text
Host Port 3000
      |
      v
Container Port 3000
