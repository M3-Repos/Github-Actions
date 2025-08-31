# GitHub Actions Mainframe JCL Deployment

This repository contains a GitHub Actions workflow that automatically deploys and executes JCL (Job Control Language) on a mainframe system.

## Overview

The workflow performs the following actions:
- Installs Zowe CLI and FTP plugin
- Uploads JCL files to the mainframe
- Submits and executes JCL jobs

## Files

- `hello-world.jcl` - Sample COBOL program that displays "HELLO ZFAM!"
- `.github/workflows/main.yml` - GitHub Actions workflow configuration

## Setup

To use this workflow, you must configure the following secrets in your GitHub repository:

- `MAINFRAME_HOST` - Mainframe hostname or IP address
- `MAINFRAME_USER` - Mainframe username
- `MAINFRAME_PASSWORD` - Mainframe password

## Configuration

The workflow triggers on:
- Push to main branch
- Manual workflow dispatch

## More Information

For detailed information about setting up GitHub secrets and configuring Zowe CLI, visit the [GitHub Actions documentation](https://docs.github.com/en/actions/security-guides/encrypted-secrets).
