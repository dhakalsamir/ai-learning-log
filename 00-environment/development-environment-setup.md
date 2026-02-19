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

## 2. Add Homebrew to PATH (Apple Silicon Macs)
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> ~/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"

## 3. Verify Homebrew installation
brew --version

## 4. Install Python
brew install python

## 5. Verify installation
python3 --version
which python3

## 6. Install VS Code
brew install --cask visual-studio-code

## 7. Verify installation
code --version

## 8. Install uv
brew install uv

## 9. Verify installation
uv --version

## 10. Create virtual environment
uv venv

## 11. Activate environment
source .venv/bin/activate
