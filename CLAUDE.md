# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Is

A personal dotfiles repository for shell prompt (Starship) and terminal emulator (Ghostty) configuration. It contains no build system, no tests, no automation scripts, and no symlink manager — files are manually deployed to their target locations.

## Repository Structure

- **`.zshrc`** — Zsh config using Oh My Zsh + plugins (git, zsh-autosuggestions, zsh-syntax-highlighting), conda initialization, Starship prompt, eza aliases, fzf integration.
- **`ghostty.config`** — Ghostty terminal emulator config: custom theme ("dankcolors"), translucent background with blur, extensive `Alt+S`-based keybindings for tabs/splits/navigation.
- **`vesper`** — Custom 16-color Ghostty palette (dark background `#101010`, warm accents).
- **`starship*.toml`** — 11 iterative Starship prompt configurations. Two palette families: Gruvbox Dark (orange/yellow) and Dracula/Nord (cyan/blue/grey). Most evolved variants: `starship_final.toml` (Dracula, Nordic grey bg) and `starship_final_battery.toml` (same + battery module).
- **`Wireshark_Config.zip`** — Exported Wireshark configuration archive.

## Config Deployment

No automation exists. Manually copy or symlink:
- `.zshrc` → `~/.zshrc`
- `starship_final.toml` (or preferred variant) → `~/.config/starship.toml`
- `ghostty.config` → `~/.config/ghostty/config`
- `vesper` → Ghostty's theme directory

## File Naming

Several filenames have typos (e.g., `startship_cyan_arrowupdare.toml`, `statship_second_gemini.toml`, `starship_orignial.toml`). These are historical and intentional — the repo doubles as an experiment log of Starship prompt iterations.
