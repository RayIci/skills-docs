# Plan & Code Review (Plannotator)

Annotate agent plans, documents and diffs, then send structured feedback back to the agent.

- [Plannotator](https://github.com/backnotprop/plannotator)
  Local, browser-based review tool for AI coding agents (Claude Code, Codex, Gemini CLI).
  Opens plans, markdown, HTML and code diffs for annotation.

  ```bash
  curl -fsSL https://plannotator.ai/install.sh | bash
  ```

  Windows PowerShell: `irm https://plannotator.ai/install.ps1 | iex`

- [Plannotator TUI](https://github.com/plannotator/plannotator-tui)
  Rust terminal app for annotating Markdown files and folders: select text, comment,
  mark sections as looks-good or delete, and send numbered feedback to your agent.

  ```bash
  brew trust plannotator/tap && brew install plannotator/tap/plannotator-tui
  # or
  cargo install plannotator-tui
  ```

- [herdr-annotate](https://github.com/plannotator/herdr-annotate)
  Plugin for [Herdr](terminal.md) to comment on terminal text and review Markdown
  documents and agent replies. Uses plannotator-tui; a "Lite" version covers terminal
  annotations only.

  ```bash
  herdr plugin install plannotator/herdr-annotate
  ```
