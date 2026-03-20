# Changelog

All notable changes to the `crrlcx.dockerized` Ansible collection will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.1.0] - 2026-03-20

### Added

- mtproxy role with configuration, tasks, and Docker Compose template

## [1.0.0] - 2026-03-20

### Added

- First stable release of the Docker role.
- Project structure and configuration files:
  - .ansible-lint, .gitattributes, .gitignore, .yamllint
- Documentation files:
  - CHANGELOG.md, README.md
- Ansible Galaxy integration files:
  - galaxy.yml, meta/runtime.yml
- Plugin documentation:
  - plugins/README.md
- Docker role features:
  - OS-based variable loading
  - Docker repository and GPG key management
  - Systemd integration for Docker prune
  - Docker registry login support
  - Python module installation for Docker
  - Customizable Docker daemon config

## [0.0.1] - 2026-03-20

### Added

- Initial project structure with configuration files:
  - .ansible-lint, .gitattributes, .gitignore, .yamllint
- Documentation files:
  - CHANGELOG.md, README.md
- Ansible Galaxy integration files:
  - galaxy.yml, meta/runtime.yml
- Plugin documentation:
  - plugins/README.md

### Other

- Initial commit
