# Nexus Registry

## Overview

Nexus Registry is a project aimed at managing and deploying container images using Docker. This repository includes configurations and scripts for setting up a registry service.

## Directory Structure

- **docker-compose.yaml**: Configuration file for Docker Compose to set up the registry service.
- **registry.conf**: Configuration file for the registry settings.

## Getting Started

### Prerequisites

- Docker installed on your system
- Docker Compose installed

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/arezoomohammadi22/nexus-registry.git
    cd nexus-registry/nexus
    ```

2. Start the registry service:
    ```bash
    docker-compose up -d
    ```

## Usage

- To push an image to your registry:
    ```bash
    docker tag [your-image] localhost:5000/[your-image]
    docker push localhost:5000/[your-image]
    ```

- To pull an image from your registry:
    ```bash
    docker pull localhost:5000/[your-image]
    ```

## Configuration

- Modify `registry.conf` to change the registry settings according to your needs.
- Update `docker-compose.yaml` if you need to customize the Docker Compose setup.

## Contributing

We welcome contributions! Please fork the repository and submit pull requests.

## License

This project is licensed under the MIT License. See the [LICENSE](../LICENSE) file for details.

## Contact

For any questions or feedback, please contact [Your Name] at [Your Email].

