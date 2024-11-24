# Development Getting Started
## Prerequisites
Ensure you have the following installed on your system:
- (Optional) [`uv`](https://docs.astral.sh/uv/)
- Python 3.9+ (preferably Python 3.13)

`uv python install 3.13` can be used to install Python 3.13 independently of the system Python version.

## Installation
1. **Clone the repository:**
    ```sh
    git clone https://github.com/JoshLoecker/mechAInistic.git
    cd mechAInistic
    ```

2. **Set up the virtual environment and install dependencies:**
    ```sh
    uv sync --python 3.13 --all-extras --dev
    ```

## Running Tests
To run the tests, use:
```sh
uv run --python 3.13 pytest --cov=tests/ --cov-report term-missing
```

## Code Formatting and Linting
This project uses `ruff` for code formatting and linting. To check the code format and linting, run:
```sh
uv run --python 3.13 ruff format --check --verbose
uv run --python 3.13 ruff check --no-fix --verbose
```

## Continuous Integration
The project uses GitHub Actions for continuous integration. The configuration is located in `.github/workflows/continuous_integration.yml`.

## Pre-commit Hooks
This project uses [pre-commit](https://pre-commit.com/) hooks to ensure code quality. To set up pre-commit hooks, run:
```sh
pre-commit install
```

## Contributing

We welcome contributions from the community! To contribute, follow these steps:

1. **Fork the repository:**
    ```sh
    git fork https://github.com/JoshLoecker/mechAInistic.git
    ```

2. **Create a new branch for your feature or bugfix:**
    ```sh
    git checkout -b {feature-or-bugfix-name}
    ```

3. **Make your changes**

4. **Commit them:**
    ```sh
    git commit -am "Description of the feature or bugfix"
    ```

5. **Push your changes to your fork:**
    ```sh
    git push origin {feature-or-bugfix-name}
    ```

6**Create a pull request:**
    Go to the original repository and create a pull request from your fork.