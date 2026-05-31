# Changelog

All notable changes to the `crrlcx.dockerized` Ansible collection will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.5.4] - 2026-05-31

### Changed

- `wgportal` role: add systemd-networkd configuration directory support.

## [1.5.3] - 2026-05-31

### Changed

- `wgportal` role: add systemd-networkd handlers and configuration for host mode.

## [1.5.0] - 2026-05-31

### Added

- New `wgportal` role with configuration, tasks, and playbooks for managing wgportal services.

## [1.4.8] - 2026-05-31

### Changed

- `docker` role: update `docker-pip` task for Python version compatibility.
- `mtproxy` role: refine secret generation method for improved security and flexibility.

## [1.4.7] - 2026-05-07

### Changed

- `telemt` role: added new logging level and improved URL handling.
- `mtproxy` role: update URL handling.

## [1.4.3] - 2026-05-07

### Changed

- `telemt` role: updated secret generation method for improved security.

## [1.4.2] - 2026-05-07

### Changed

- `telemt` role: updated defaults and tasks for improved configuration and secret handling.

## [1.4.0] - 2026-05-06

### Added

- New `telemt` role with configuration, tasks, and playbooks for managing telemt services.

## [1.3.11] - 2026-05-06

### Changed

- `cloudflared`, `mtproxy`, and `zerotier` roles: updated to create config files from templates.

## [1.3.8] - 2026-04-27

### Changed

- `docker` role: default `docker_version` updated to `29.4.1`
- `docker` role: added `docker_compose_version` default (`5.1.3`)
- `docker` role: `docker-compose-plugin` install now uses pinned `docker_compose_version` variable

## [1.3.7] - 2026-03-21

### Added

- Destructors for cloudflared, mtproxy, and zerotier roles added to remove Docker containers and configurations

### Changed

- **BREAKING:** Playbooks for cloudflared, mtproxy, and zerotier roles renamed to match role names
- `mtproxy` role: secret generation now uses a Jinja2 loop for flexible secret count

## [1.3.5] - 2026-03-21

### Fixed

- Fix zerotier data directory variable by adding missed datacenter and timezone defaults

## [1.3.4] - 2026-03-21

### Added

- New zerotier role with configuration, tasks, and Docker Compose template

### Changed

- Update docker-compose templates to check length of hosts dictionary instead of existence of variable

### Fixed

- Fix docker-compose templates to use correct variable names for mtproxy and cloudflared

## [1.2.1] - 2026-03-20

### Added

- New cloudflared role with configuration, tasks, and Docker Compose template

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

- New mtproxy role with configuration, tasks, and Docker Compose template

## [1.0.0] - 2026-03-20

### Added

- First stable release of the Docker role.
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
