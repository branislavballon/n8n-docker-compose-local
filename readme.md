# n8n Docker Compose Local Setup

A simple Docker Compose configuration for running the n8n automation tool locally.
This setup allows you to start and stop n8n with short commands, making it easier to experiment without a lengthy docker command.

## Basic Information

- Official documentation: [n8n Docs](https://docs.n8n.io/)
- Local data is stored in the `n8n_data` directory alongside this repository.
- Based on the official guide: [Docker Compose Setup](https://docs.n8n.io/hosting/installation/server-setups/docker-compose/#6-create-docker-compose-file)
- **Note:** This is **not** intended for production use. Please refer to the official documentation for production-ready configurations.

## Getting Started

1. **Install Docker:**

   Make sure Docker is installed and running on your system.
   [Install Docker](https://docs.docker.com/get-docker/)

1. **Clone this repository:**

    ```bash
    git clone git@github.com:branislavballon/n8n-docker-compose-local.git
    ```

1. **Navigate to the project directory:**

    ```bash
    cd n8n-docker-compose-local
    ```

1. **(Optional) Grant execute permissions to the start and stop scripts:**

    ```bash
    chmod u+x ./start.sh ./stop.sh
    ```

1. **Start the application:**

    ```bash
    ./start.sh
    ```

1. **Stop the application:**

    ```bash
    ./stop.sh
    ```

### Commands Overview

- Start n8n: `./start.sh` This runs the Docker Compose configuration in detached mode.
- Stop n8n: `./stop.sh` This stops the container defined in the Docker Compose configuration.

### Notes

- If you encounter permission issues, ensure the start.sh and stop.sh scripts are executable: `chmod u+x ./start.sh ./stop.sh`

- Data persistence: The n8n_data directory holds all data and configurations. Make sure to back up this directory if you plan to move your environment.

- For further details, refer to the official n8n documentation:
n8n Docs (https://docs.n8n.io/)
