# LLM From Scratch Setup Guide

This document provides step-by-step instructions to set up the development environment for the LLM From Scratch project.

## Environment and Package Management with uv

We use `uv` for creating a virtual environment and for fast, efficient package installation. It's an extremely fast Python package installer and resolver, written in Rust.

### 1. Install uv

If you don't have `uv` installed, you can install it using this command:

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

Follow the instructions on the screen to add `uv` to your shell's configuration file.

### 2. Create a Virtual Environment

Once `uv` is installed, create a new virtual environment for this project. This will create a `.venv` directory in the project folder.

```bash
uv venv
```

### 3. Activate the Environment

Before you start working on the project, you need to activate the virtual environment.

```bash
source .venv/bin/activate
```

Your terminal prompt should now show that you are in the `.venv` environment.

### 4. Install Project Dependencies

All required Python packages are listed in the `requirements.txt` file. Use `uv` to install them into your active environment:

```bash
uv pip install -r requirements.txt
```

This ensures you have all the necessary libraries to run the code in this project. 