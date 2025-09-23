# Cadmus FeBo API

- [models](https://github.com/vedph/cadmus-febo)
- [app](https://github.com/vedph/cadmus-febo-app)

API service for Cadmus [FeBo](https://erc-febo.unitn.it) (_Federalism and Border Management in Greek Antiquity_).

🐋 Quick Docker image build (you need to have a `buildx` container):

```bash
docker buildx create --use

docker buildx build . --platform linux/amd64,linux/arm64,windows/amd64,windows/arm64 -t vedph2020/cadmus-febo-api:2.0.0 -t vedph2020/cadmus-febo-api:latest --push
```

(replace with the current version).

This is a Cadmus API layer customized for the PRJ project. Most of its code is derived from shared Cadmus libraries.

## History

- 2025-09-23: updated packages.
- 2025-06-03: updated packages.

### 2.0.0

- 2025-05-09:
  - ⚠️ updated packages (epigraphic models).
  - updated preview profile.
  - updated profile.

### 1.0.5

- 2025-02-19: added `.AddApplicationPart(typeof(ThesaurusImportController).Assembly)`.

### 1.0.4

- 2025-02-18: updated packages.
- 2025-01-28: updated packages.

### 1.0.3

- 2025-01-23: updated packages.
- 2025-01-19: updated packages.
- 2025-01-01: updated packages.
- 2024-12-23: updated packages.

### 1.0.2

- 2024-12-21: updated packages.
- 2024-12-16: updated packages.
- 2024-12-03: updated packages.
- 2024-11-30: updated packages.

### 1.0.1

- 2024-11-29: updated packages.

### 1.0.0

- 2024-11-23: ⚠️ upgraded to .NET 9.
- 2024-09-30: updated packages.

### 0.0.3

- 2024-07-24: updated packages.
- 2024-07-19: updated packages.
- 2024-07-15: updated packages.
- 2024-07-08: updated packages.
- 2024-06-30: updated packages.
- 2024-06-24:
  - updated packages.
  - added epigraphic parts for fragments and signs.
- 2024-06-22: replaced historical datation part with chronotopes in inscription facet.
- 2024-06-09: updated packages.
- 2024-05-23: updated packages.
- 2024-05-11: added proxy.
- 2024-05-02: updated packages.

### 0.0.2

- 2024-04-11: updated packages.

### 0.0.1

- initial release.
