# OpenClaw + LM Studio (Local)

Run OpenClaw against a local LLM served by [LM Studio](https://lmstudio.ai), with optional GitHub integration.

## Prerequisites

- Windows 10/11
- [LM Studio](https://lmstudio.ai) with a chat/instruct model loaded
- Node.js 22+ (v26 works)
- Git and GitHub CLI (`gh`)

## Quick start

1. Start LM Studio local server (default: `http://localhost:1234`).
2. Install OpenClaw: `npm install -g openclaw@latest`
3. Run onboarding: `openclaw onboard`
4. Choose **LM Studio** and pick your model.

See [docs/setup.md](docs/setup.md) for the full step-by-step guide.

## Use on all your devices

GitHub is the source of truth. On each new machine (once):

```bash
git clone https://github.com/Hernashi/openclaw-lmstudio.git
```

Then in Cursor: **File → Open Folder** → select the cloned folder.

To get the latest changes on any device:

```bash
git pull
```

## Security

- Never commit `.env`, tokens, or `.openclaw/` auth files.
- Use `gh auth login` for GitHub instead of storing tokens in config when possible.
- Copy `config/openclaw.example.json` as a reference only; OpenClaw writes live config to `~/.openclaw/` during onboarding.

## License

MIT
