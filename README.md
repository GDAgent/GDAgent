# GDAgent

GDAgent is an AI development environment for Godot. It brings terminal-based coding agents directly into the editor, so you can work from your current project root without bouncing between Godot, browser tabs, and external terminals.

It is built around a native terminal workflow inside Godot: workspace restore, multi-agent layouts, fast setup, and tools that stay attached to the project you are actually working on.

## Highlights

- Native terminal workspace inside Godot
- Workspace restore across editor restarts
- Split and multi-agent layouts
- First-run setup that detects supported AI CLIs
- Prompt templates for common Godot tasks
- Bundled Godot MCP integration for supported agents

## Supported Tools

GDAgent works with:

- Claude Code
- Google Antigravity CLI
- Aider
- GitHub Copilot CLI
- Mistral Vibe
- OpenAI Codex CLI
- OpenCode

## Install

Requirements:

- Godot 4.6+
- Windows 11 or Linux x86_64

Install flow:

1. Download `gdagent` for your platform.
2. Launch it and activate your license.
3. Select a Godot project and click **Install**.
4. Open the project in Godot and start a new agent tab.

## Notes

- GDAgent runs locally on your machine.
- You bring your own API keys or subscriptions for the AI tools you use.

## Release Verification (Linux)

We sign all our Linux releases with a GPG key. If you want to manually verify the integrity of the downloaded archive before installing:

1. Import our official GPG public key from the Ubuntu keyserver:
   ```bash
   gpg --keyserver keyserver.ubuntu.com --recv-keys <INSERT_YOUR_KEY_ID_HERE>
   ```
2. Download both the release archive (e.g., `gdagent-v1.0.0-linux.tar.gz`) and the signature file (`gdagent-v1.0.0-linux.tar.gz.asc`) into the same folder.
3. Verify the signature:
   ```bash
   gpg --verify gdagent-v1.0.0-linux.tar.gz.asc gdagent-v1.0.0-linux.tar.gz
   ```
   *You should see a message indicating a "Good signature" from the GDAgent Team.*

## Links

- Website: <https://gdagent.dev>
- Docs: <https://gdagent.dev/docs>
- Issues: <https://github.com/GDAgent/GDAgent/issues>
