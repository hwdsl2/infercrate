# Changelog

Notable changes to InferCrate are documented here.

## 2026-11-15

Release: `2026.11.1`

### Added

- Accept mounted secret files through `OLLAMA_API_KEY_FILE` with explicit source-conflict and file validation.

### Compatibility

- Rotation applies at startup. Existing direct/generated credentials and volumes remain supported; older images require an older supported credential source.
- Existing persisted/shared credentials and upstream settings remain in use; file inputs do not automatically rotate saved secondary credentials.

## 2026-11-10

### Changed

- Verify Caddy release checksums before extraction in CPU and CUDA builds
  while retaining latest-release discovery.

## 2026-10-24

Release: `2026.10.1`

### Changed

- Established the first tagged source release. Docker images continue to update
  independently through existing moving tags.

## 2026-10-09

### Changed

- Rebranded as InferCrate (formerly `docker-ollama`); the Docker image name
  remains `hwdsl2/ollama-server`.

## 2026-07-09

### Added

- Added anonymous aggregate deployment/upgrade counts. Opt out with
  `OLLAMA_DISABLE_USAGE_COUNTS=1`.

## Earlier notable changes

- Added an authenticated Ollama endpoint with automatic key generation,
  persistent models, model-management commands, and API key sharing with
  stack services.
- Added CPU and NVIDIA CUDA images with automatic model downloads on first
  start.
