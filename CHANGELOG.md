# Changelog

Notable changes to InferCrate are documented here.

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
