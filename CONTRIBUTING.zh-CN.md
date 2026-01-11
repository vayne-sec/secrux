# 贡献指南

欢迎参与 Secrux 的开发与改进！

## 仓库拉取

本仓库使用 Git submodule 管理核心模块：

```bash
git clone --recurse-submodules <YOUR_REPO_URL>
```

如果你已经克隆但忘记初始化 submodule：

```bash
git submodule update --init --recursive
```

## 开发与测试

- `secrux-server`（Kotlin/Spring Boot）：`./gradlew bootRun`、`./gradlew test`
- `secrux-web`（Vite/React）：`npm install`、`npm run dev`、`npm run build`
- `secrux-ai`（Python/FastAPI）：参考 `secrux-ai/README.zh-CN.md`
- `secrux-executor`（Go）：`go test ./...`、`go build`
- `secrux-engine`（引擎镜像/脚本）：参考 `secrux-engine/README.zh-CN.md`

## PR 提交建议

- 改动尽量聚焦，并补齐文档说明。
- 不要提交敏感信息（`.env`、token、私钥等）。
- 建议使用 `<type>: <imperative summary>` 的提交信息格式（例如：`fix: xxx`）。
