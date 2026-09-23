# Cadmus FeBo API

- [models](https://github.com/vedph/cadmus-febo)
- [app](https://github.com/vedph/cadmus-febo-app)

API service for Cadmus [FeBo](https://erc-febo.unitn.it) (_Federalism and Border Management in Greek Antiquity_).

🐋 Quick Docker image build (you need to have a `buildx` container):

Before creating Docker images, ensure you have a buildx builder instance running that supports multi-arch:

```sh
docker buildx create --use --name multi-arch-builder || docker buildx use multi-arch-builder
docker buildx inspect --bootstrap
```

Build:

```bash
docker buildx build --platform linux/amd64,linux/arm64 -t vedph2020/cadmus-febo-api:4.0.4 -t vedph2020/cadmus-febo-api:latest --push .
```

(replace with the current version).

This is a Cadmus API layer customized for the PRJ project. Most of its code is derived from shared Cadmus libraries.

## Parts Matrix

|               | inscription      | passage          | conflict | actor |
| ------------- | ---------------- | ---------------- | -------- | ----- |
| categories    | ins-fn topic     | topic            | topic    | actor |
| comment       |                  |                  | X        |       |
| date          | document episode | document episode | X        |       |
| keywords      | X                | X                | X        | X     |
| links         | X                | X                | X        | X     |
| metadata      | X                | X                | X        | X     |
| names         |                  |                  |          | X     |
| note          | X trans          | X trans          | X        | X     |
| references    | X                | X                | X        | X     |
| scripts (EPI) | X                |                  |          |       |
| support (EPI) | X                |                  |          |       |
| text          | X                | X                |          |       |
| apparatus=    | X                | X                |          |       |
