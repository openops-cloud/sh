# AGENTS.md

## Repository Purpose

This repository contains a collection of shell scripts for **OpenOps**, designed to be executed remotely via `curl` piping. These scripts enable users to quickly perform operations without needing to clone the repository or manually download files.

## Content

The `scripts/` directory contains utility scripts including:
- `install` - Installation script for OpenOps
- `help` - Help and documentation script
- `share-logs` - Log sharing utility
- `tls` - TLS-related operations

## Key Requirements

### POSIX Compliance

All scripts in this repository **must be POSIX-compliant**. This ensures:
- Maximum portability across different Unix-like systems
- Compatibility with various shell implementations (sh, dash, bash, etc.)
- Reliability when executed in minimal environments

### Remote Execution

Scripts are designed to be piped directly from the web:

```shell
curl -fsS https://openops.sh/install | sh
```

This means scripts must:
- Be safe for direct execution
- Handle environment variables appropriately
- Provide clear error messages
- Exit cleanly on errors

## Usage

See [openops.sh/help](https://openops.sh/help) and [docs.openops.com](https://docs.openops.com) for complete documentation and usage examples.
