# flexget-check-github-action

A GitHub Action to check a FlexGet config.

Example:
```
name: Check flexget config

on:
  push:

jobs:
  check-config:
    runs-on: ubuntu-latest
    steps:
    - name: Checkout code
      uses: actions/checkout@v3
    - name: Set up Python
      uses: actions/setup-python@v4
    - name: Check flexget config
      uses: narumiruna/flexget-check-action@v0.1.1
```