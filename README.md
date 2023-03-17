# EEG Analysis with Matlab in Docker Containers
This repository contains scripts and resources for setting up and running multiple instances of Matlab in Docker containers, specifically optimized for high volume EEG analysis labs. By leveraging Docker and Matlab, users can efficiently utilize resources, collaborate easily, and streamline their EEG analysis workflows.

## Features
Run multiple Matlab instances on a single computer
Access Matlab instances through a web browser
GPU passthrough and configurable memory/CPU sharing
Flexible Matlab licensing
Easy setup, cloning, and modification of instances using Docker Compose

## Prerequisites
Docker and Docker Compose installed on your system
Matlab base image from Mathworks (mathworks/matlab-deep-learning:r2021b or any suitable image)
Access to Matlab license servers for the required licenses (academic network, student, or professional)

## Setup
Clone this repository to your local machine:
```bash
git clone https://github.com/yourusername/eeg-analysis-matlab-docker.git
cd eeg-analysis-matlab-docker
```

Replace the placeholders in the .env file with your specific values:
https://docs.docker.com/compose/environment-variables/set-environment-variables/

```bash
CONTAINERNAMEA=<container_name_A>
CONTAINERNAMEB=<container_name_B>
...
LICENSE_SERVER=<license_server>
```

Activate docker compose:
```bash
docker-compose up
```

Access the running Matlab instances through your web browser using the specified web ports (e.g., <web_port_A>).
