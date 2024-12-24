# Containerised nlp

A quick and easy setup for running Jupyter NLP notebooks in a Dockerized environment, managed using [Docker Compose](https://docs.docker.com/compose/). This setup makes it simple to get up and running with Jupyter and LLMs, share notebooks across multiple team members, and maintain consistent environments. 

## Features

- Dockerized Jupyter environment for consistent, reproducible NLP development.
- Simplified sharing of notebooks using the `work` directory.

## Getting Started

Clone this repository to your local machine:

```bash
git clone https://github.com/tmnestor/containerised_nlp
```

Navigate to the project root directory.

Build the the image for the Jupyter Notebook server:

```bash
docker compose build
```

Start the Jupyter Notebook server:

```bash
docker compose up
```

After running this command, the Jupyter Notebook server should be accessible at `http://localhost:8888`.

## Directory Structure

- `./work`: This is the directory where you can add your Jupyter notebooks. It's mounted as a volume in the Docker container, so notebooks created and saved in the Jupyter Notebook IDE will persist here.

## Notes

The `requirements.txt` file is copied to the Docker container during the build process, and the Python dependencies listed within are installed. To add or update dependencies, modify this file, then rebuild the Docker image.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
