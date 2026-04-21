# skills

Installable OpenClaw/Codex skills published from this repository.

## Included Skills

- `crypto-news-http-api` - Call the Crypto News Analyzer HTTP API for async analysis jobs, semantic search, datasource management, and health checks.

## Install

Install a tagged release instead of `main` so behavior stays stable:

```bash
python3 install-skill-from-github.py \
  --repo LaceLetho/skills \
  --path skills/crypto-news-http-api \
  --ref v0.1.0
```

You can also install from a GitHub URL:

```bash
python3 install-skill-from-github.py \
  --url https://github.com/LaceLetho/skills/tree/v0.1.0/skills/crypto-news-http-api
```

## Upgrade

The current installer copies the skill into `$CODEX_HOME/skills/<skill-name>` and aborts if that directory already exists. Upgrade by removing the old copy, then reinstalling the new tagged version:

```bash
rm -rf ~/.codex/skills/crypto-news-http-api
python3 install-skill-from-github.py \
  --repo LaceLetho/skills \
  --path skills/crypto-news-http-api \
  --ref v0.1.0
```

When you publish a new version, replace `v0.1.0` with the newer tag such as `v0.2.0`.
