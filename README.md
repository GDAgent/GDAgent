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
- Grok Build
- Command Code

You can also add any other agent CLI under **Settings > Agents** by giving it a name and a command.

## Install

Requirements:

- Godot 4.6+
- Windows 11 or Linux x86_64 (macOS is planned)

Install flow:

1. Download the `gdagent` archive for your platform (`.zip` for Windows, `.tar.gz` for Linux) from the links in your purchase email.
2. Launch it and activate your license. Each license allows 2 simultaneous activations.
3. Select a Godot project and click **Install**.
4. Open the project in Godot and start a new agent tab.

## Notes

- GDAgent runs locally on your machine.
- You bring your own API keys or subscriptions for the AI tools you use.

## Release Verification (Linux)

We sign all our Linux releases with a GPG key. If you want to manually verify the integrity of the downloaded archive before installing:

1. Import our official GPG public key from the Ubuntu keyserver:
   ```bash
   gpg --keyserver keyserver.ubuntu.com --recv-keys 133C562637EE5390103D48A43B39EF48E35311DE
   ```
2. Download both the release archive (e.g., `gdagent-v1.0.0-linux.tar.gz`) and the signature file (`gdagent-v1.0.0-linux.tar.gz.asc`) into the same folder. Both are in the download links from your purchase email.
3. Verify the signature:
   ```bash
   gpg --verify gdagent-v1.0.0-linux.tar.gz.asc gdagent-v1.0.0-linux.tar.gz
   ```
   *You should see a message indicating a "Good signature" from the GDAgent Team.*

If you don't have GPG installed, you can check the archive's integrity against the `.sha256` file from the same email instead:

```bash
sha256sum -c gdagent-v1.0.0-linux.tar.gz.sha256
```

*You should see an "OK" message if the file is intact.*

## Links

- Website: <https://gdagent.dev>
- Docs: <https://gdagent.dev/docs>
- Issues: <https://github.com/GDAgent/GDAgent/issues>
