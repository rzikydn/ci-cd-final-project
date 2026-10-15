# CI/CD Tools and Practices Final Project

## Project Details
- **Project Name:** `ci-cd-final-project`
- **Course:** Continuous Integration and Continuous Delivery (CI/CD)
- **Author:** rzikydn
- **Platform:** Coursera / IBM Developer Skills Network

## Overview
This repository contains the full CI/CD pipeline implementation for the final project. It demonstrates automated continuous integration using GitHub Actions (Linting with `flake8` and unit testing with `nose`) and continuous delivery using Tekton Pipelines on OpenShift (`cleanup`, `git-clone`, `flake8`, `nose`, `buildah`, `deploy`).

## Project Structure
- `.github/workflows/workflow.yml`: GitHub Actions CI pipeline configuration
- `.tekton/tasks.yml`: Tekton custom tasks definitions (`cleanup` and `nose`)
- `service/`: Flask application microservice
- `tests/`: Unit test suite executed via `nosetests`
- `Dockerfile`: Container image configuration for building with Buildah / Podman
- `requirements.txt`: Python package dependencies

## License
Licensed under the Apache License 2.0.
