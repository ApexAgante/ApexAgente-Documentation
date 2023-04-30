---
title: Getting Started
---
# Getting Started
---
## Importing

- CLI
```sh
git clone -b cli https://github.com/ApexAgante/ApexAgente
```

- GUI
```sh
git clone -b gui https://github.com/ApexAgante/ApexAgente
```

## Installation

### Directory
Go to your project directory by using:
``` bash
cd ApexAgente
```

### Environment <small>optional</small> { #environment }
We recommend using a [virtual environment](https://realpython.com/what-is-pip/#using-pip-in-a-python-virtual-environment), which is an isolated Python runtime. If you are in a virtual environment, any packages that you install or upgrade will be local to the environment. If you run into problems, you can just delete and recreate the environment. It's trivial to set up:

??? poetry "poetry (strongly recommended)"
    - Poetry automatically created virtual environment

    - Activate the environment with:
        ``` sh
        poetry shell
        ```

    - Exit your virtual environment using:
        ``` bash
        exit
        ```

??? pipenv "pipenv (recommended)"
    - Pipenv automatically created virtual environment

    - Activate the environment with:
        ``` sh
        pipenv shell
        ```

    - Exit your virtual environment using:
        ``` bash
        exit
        ```

??? python "pip"

    - Create a new virtual environment
        ``` bash
        python3 -m venv venv
        ```
    - Activate the environment with:
        ``` sh
        . venv/bin/activate (Linux / MacOS) / venv/Scripts/activate (Windows)
        ```
    - Exit your virtual environment using:

        ``` sh
        deactivate
        ```

### Dependencies Installation
Apex Agente has several dependencies that can be installed with
`poetry` or `pipenv` or `pip`, ideally by using a [virtual environment](https://docs.python.org/3/library/venv.html). Open up a terminal and install all dependencies with:

- **poetry**

    ```sh
    poetry install
    ```

- **pipenv**

    ```sh
    pipenv sync
    ```

- **pip**

    ```sh
    pip install -r requirements.txt
    ```

This will automatically install compatible versions of all dependencies. ApexAgente always strives to support the latest versions, so there's no need to install those packages separately.

## Run Locally

To run it locally is pretty simple, just run it with:

- **poetry**
    
    ``` sh
    poetry run app [--api API KEY] [--id APPLICATION ID] [--url SERVER URL] [--n DEFAULT CONFIGURATION]
    ```

- **poetry**

    ``` sh
    pipenv run app [--api API KEY] [--id APPLICATION ID] [--url SERVER URL] [--n DEFAULT CONFIGURATION]
    ```

- **python3**

    ``` sh
    python3 -m app/main.py [--api API KEY] [--id APPLICATION ID] [--url SERVER URL] [--n DEFAULT CONFIGURATION]
    ```

??? info "Information"

    - The `--api` option specifies api key used in the application.
    - The `--id` option specifies application id used in the application.
    - The `--url` option serves as base url for the application.
    - The `--n` options determine whether using the options or use default configuration. If you use `--n` you do not need to use other options
    
    *Note: The program can be run without the need for the user to specify any options.*

## Usage Example

![Run](assets/terminal.svg)