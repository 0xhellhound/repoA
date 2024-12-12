# Malicious Action

This repository contains a vulnerable GitHub Action that demonstrates potential security issues in CI/CD pipelines.

## Features
- Simulates a malicious action capable of exfiltrating sensitive data and propagating to dependent repositories.
- Provides a starting point for understanding the impact of insecure GitHub Actions.

## Usage
Add the following workflow to your repository to use this action:

```yaml
name: Use Malicious Action
on: push
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - name: Run Malicious Action
        uses: <owner>/repo-a@main
```
