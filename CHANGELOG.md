# Changelog

All notable changes to the `crrlcx.dockerized` Ansible collection will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.2.1] - 2026-03-20

### Added

- cloudflared role with configuration, tasks, and Docker Compose template

### Changed

- Update mtproxy role: hosts file variable should be a dictionary, not a list

## [1.1.2] - 2026-03-20

### Changed

- Update mtproxy role with secret generation and configuration improvements

### Removed

- Remove unused docker template variables

### Fixed

- Fix docker-prune-off task to prevent failure when timer is not found

## [1.1.0] - 2026-03-20

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
