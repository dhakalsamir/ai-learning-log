# macOS AI/ML Development Environment Setup

## Overview

Before building AI/ML systems, a clean and reproducible development environment must be established.

A computer operates as:

Input → Process → Output

When running Python:

Terminal → Python Interpreter → Operating System → CPU + RAM → Output

Understanding this stack makes environment setup intentional rather than mechanical.

---

## 1. Install Homebrew (macOS Package Manager)

/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

## Add Homebrew to PATH (Apple Silicon Macs)
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> ~/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"

## Verify Homebrew installation
brew --version

## Install Python
brew install python

## Verify installation
python3 --version
which python3

## Install VS Code
brew install --cask visual-studio-code

## Verify installation
code --version

## Install uv
brew install uv

## Verify installation
uv --version

## Create virtual environment
uv venv

## Activate environment
source .venv/bin/activate
