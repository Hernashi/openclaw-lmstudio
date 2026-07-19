# Setup guide: OpenClaw + LM Studio on Windows

## Step 1 — LM Studio

1. Open LM Studio.
2. Load a chat/instruct model (50k+ context recommended for agent tools).
3. Start the local server on port **1234**.

Verify:

```powershell
curl http://localhost:1234/api/v1/models
```

## Step 2 — Install OpenClaw

```powershell
npm install -g openclaw@latest
openclaw onboard --install-daemon
```

## Step 3 — Connect GitHub

```powershell
gh auth login
```

## Step 4 — Use on other devices

Clone this repo on the other machine, install LM Studio + OpenClaw, then run `openclaw onboard` again.
