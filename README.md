# skills

Installable OpenClaw skills published from this repository.

## Included Skills

- `crypto-news-http-api` - Call the Crypto News Analyzer HTTP API for async analysis jobs, semantic search, datasource management, and health checks.

## Install In OpenClaw

OpenClaw loads skills from `<workspace>/skills`, `<workspace>/.agents/skills`, `~/.agents/skills`, and `~/.openclaw/skills`. Until this skill is published on ClawHub, install it by copying the versioned skill directory from this repo into one of those locations.

Shared install for all local OpenClaw workspaces:

```bash
git clone --branch <tag> --depth 1 https://github.com/LaceLetho/skills.git
mkdir -p ~/.openclaw/skills
cp -R skills/skills/crypto-news-http-api ~/.openclaw/skills/
```

Workspace-local install:

```bash
git clone --branch <tag> --depth 1 https://github.com/LaceLetho/skills.git
mkdir -p ./skills
cp -R skills/skills/crypto-news-http-api ./skills/
```

Start a new OpenClaw session after installing or updating the skill so the new snapshot is loaded.

Replace `<tag>` with a released version such as `v0.2.0`.

## Upgrade

Replace the existing `crypto-news-http-api` directory with a newer tagged copy from this repo, then start a new OpenClaw session.

Once the skill is published to ClawHub, the native OpenClaw path becomes:

```bash
openclaw skills install crypto-news-http-api
openclaw skills update --all
```
