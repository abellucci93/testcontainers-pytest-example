# Testcontainers Pytest Example

See https://testcontainers.com/guides/getting-started-with-testcontainers-for-python/

A Python project demonstrating integration testing with pytest and Testcontainers, using Docker-based ephemeral services and mise for runtime management.

## Requirements

* Docker (running locally)
* mise

## Setup

1. Install tool versions using the local `mise.toml` file.

```sh
mise install
```

2. Create python virtual environment

```sh
python -m venv venv
```

3. Activate python virtual environment

```sh
source venv/bin/activate
```

4. Install dependencies

```sh
pip install -r requirements.txt
```

## Running Tests

Make sure Docker is running, then execute:

```sh
pytest -v
```

Testcontainers will automatically start and stop required Docker containers during the test session.

