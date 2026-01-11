# Disclaimer

Secrux is an open-source security governance platform intended for **defensive security** and **authorized** use only.

## Scope of use

- Use Secrux only on assets you own, or where you have explicit permission to scan and analyze.
- Scan results may contain false positives/negatives and should be reviewed by qualified personnel.

## AI, privacy, and sensitive data

Secrux can integrate with external LLM providers if configured. Depending on your configuration, **source code, logs, findings, and metadata** may be sent to that provider.

- If you handle sensitive data (secrets, proprietary code, regulated data), prefer **local/self-hosted** models and keep all services within your trusted network.
- If you cannot accept any data egress, disable online LLM calls by leaving `SECRUX_AI_LLM_BASE_URL` / `SECRUX_AI_LLM_API_KEY` / `SECRUX_AI_LLM_MODEL` empty.
- Treat tokens, credentials, and prompt dumps as sensitive. Keep `SECRUX_AI_PROMPT_DUMP=off` in production.

You are responsible for evaluating and complying with your organization’s data handling policies and applicable laws/regulations.

## No warranty / limitation of liability

Secrux is provided **“AS IS”**, without warranty of any kind, express or implied. To the maximum extent permitted by law, the maintainers and contributors are not liable for any damages or losses arising from the use (or inability to use) the software.
