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

## Cross-device access

Cursor account sync keeps **settings and rules**, not project folders. To use this project on another machine:

```bash
git clone https://github.com/YOUR_USERNAME/openclaw-lmstudio.git
cd openclaw-lmstudio
```

Then open the folder in Cursor and continue setup on that machine.

## Security

- Never commit `.env`, tokens, or `.openclaw/` auth files.
- Use `gh auth login` for GitHub instead of storing tokens in config when possible.
- Copy `config/openclaw.example.json` as a reference only; OpenClaw writes live config to `~/.openclaw/` during onboarding.

## License

MIT
