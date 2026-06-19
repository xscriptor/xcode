# Security Policy

## Reporting a Vulnerability

If you discover a security vulnerability in this project, please open an issue on the repository describing the finding. Do not disclose the vulnerability publicly until it has been addressed.

This project distributes Xcode theme files (`.xccolortheme`) and a Python generator script. These files do not execute arbitrary code and present minimal security risk, but we still appreciate responsible disclosure of any potential issues.

## Scope

- The Python generator (`labs/generate_themes.py`)
- Distribution scripts (`install.sh`)
- Any configuration files that affect system state

## Out of Scope

- Third-party dependencies (please report to the respective maintainers)
- Xcode itself (contact Apple via their security portal)
