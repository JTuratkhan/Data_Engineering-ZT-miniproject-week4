[![Python Matrix Build](https://github.com/JTuratkhan/ZT-miniproject-week4/actions/workflows/cicd.yml/badge.svg?branch=main)](https://github.com/JTuratkhan/ZT-miniproject-week4/actions/workflows/cicd.yml)

## ZT-miniproject-week4

# Setting up a Repo and adding a Python Project
Let's consider a simple Python project that should run on different versions of Python. This project has a file names 'main.py' and a file names 'test_main.py' for testing.

# GitHub Actions Workflow
In .github folder, you can see workflows folder. Inside the directoru, yml file was created with configurations that run whenever there's a push to the 'main' branch. It uses matrix strategy to test against Python 3.7, 3.8 and 3.9. It checks out the code, sets up the necessary Python version, installs the dependencies (if any), and runs tests.
""" strategy:
      matrix:
        python-version: [3.7, 3.8, 3.9]  # Add or remove versions as needed"""
