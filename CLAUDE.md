# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Is

A personal dotfiles repository for shell prompt (Starship) and terminal emulator (Ghostty) configuration. It contains no build system, no tests, no automation scripts, and no symlink manager — files are manually deployed to their target locations.

## Repository Structure

- **`.zshrc`** — Zsh config using Oh My Zsh + plugins (git, zsh-autosuggestions, zsh-syntax-highlighting), conda initialization, Starship prompt, eza aliases, fzf integration.
- **`ghostty.config`** — Ghostty terminal emulator config: custom theme ("dankcolors"), translucent background with blur, extensive `Alt+S`-based keybindings for tabs/splits/navigation.
- **`vesper`** — Custom 16-color Ghostty palette (dark background `#101010`, warm accents).
- **`starship.toml`** — Primary Starship prompt config using Catppuccin Mocha palette with powerline segments. Includes all dev modules: 15 languages, git (branch/commit/status/metrics), cloud (AWS, GCP, Kubernetes), Docker, Conda, Nix, battery, memory, cmd_duration, jobs. Requires a Nerd Font patched font.
- **`starship_*.toml`** — Historical Starship variants (Gruvbox, Dracula/Nord palettes). Kept as experiment log, not active configs.
- **`Wireshark_Config.zip`** — Exported Wireshark configuration archive.

## Config Deployment

No automation exists. Manually copy or symlink:
- `.zshrc` → `~/.zshrc`
- `starship.toml` → `~/.config/starship.toml`
- `ghostty.config` → `~/.config/ghostty/config`
- `vesper` → Ghostty's theme directory

## File Naming

Several filenames have typos (e.g., `startship_cyan_arrowupdare.toml`, `statship_second_gemini.toml`, `starship_orignial.toml`). These are historical and intentional — the repo doubles as an experiment log of Starship prompt iterations.
