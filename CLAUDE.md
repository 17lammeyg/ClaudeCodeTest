# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repo is

A demonstration repository for showcasing Claude Code capabilities to clients. It contains two discrete demo artifacts:

- **Demo 1 — Game build:** `tictactoe.html`, a self-contained browser game built by Claude Code to show rapid UI generation.
- **Demo 2 — Consulting AI workflow:** `demo_data/` contains a consulting client brief (`client_brief.txt`), the prompt used to drive analysis (`demo2_prompt.txt`), and Claude's structured output (`framework_output.md`), demonstrating Claude Code applied to knowledge work.

## Running the project

There is no build system, package manager, or server. Everything runs directly in a browser:

- Open `tictactoe.html` in any browser to play the game.
- The `demo_data/` files are plain text/markdown — view in any editor or browser.

## Architecture

`tictactoe.html` is a single-file app — all HTML, CSS, and JS are inline. Game state is held in module-level variables (`board`, `current`, `gameOver`, `score`). The win-check logic iterates over the `WINS` constant (8 winning index triplets). There is no framework, bundler, or external dependency.

`demo_data/framework_output.md` is the output artifact from Demo 2 and is meant to be read alongside `client_brief.txt` to show the full input-to-output arc of an AI-assisted consulting workflow.

## Git workflow

All changes should be committed with clear, descriptive messages and pushed to `origin/master` (GitHub: `17lammeyg/ClaudeCodeTest`) so there is always a recoverable snapshot.
