# Contributing

Thanks for contributing to Secrux!

## Repository setup

This repo uses Git submodules for core modules:

```bash
git clone --recurse-submodules <YOUR_REPO_URL>
```

If you already cloned without submodules:

```bash
git submodule update --init --recursive
```

## Development

- `secrux-server` (Kotlin/Spring Boot): `./gradlew bootRun`, `./gradlew test`
- `secrux-web` (Vite/React): `npm install`, `npm run dev`, `npm run build`
- `secrux-ai` (Python/FastAPI): see `secrux-ai/README.md`
- `secrux-executor` (Go): `go test ./...`, `go build`
- `secrux-engine` (engine images/scripts): see `secrux-engine/README.md`

## Pull requests

- Keep changes focused and documented.
- Do not commit secrets (`.env`, tokens, private keys).
- Prefer commit messages like `<type>: <imperative summary>` (e.g. `fix: handle empty tenant header`).
