<div align="center">

# 🌍 i18n-localizer

**AI-powered internationalization and localization for web, mobile, and native Apple apps.**

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Claude Code](https://img.shields.io/badge/Claude_Code-Skill-blueviolet)](https://docs.anthropic.com/en/docs/claude-code)
[![Languages](https://img.shields.io/badge/Languages-47+-green.svg)](#what-it-does)

A [Claude Code](https://docs.anthropic.com/en/docs/claude-code) skill that enables Claude to scan your codebase for translatable strings, set up i18n infrastructure, generate high-quality localized translations, handle SEO metadata, and maintain translation files — all without external API calls.

</div>

---

## ⚡ Quick Start

```bash
git clone https://github.com/hacksurvivor/i18n-localizer.git ~/.claude/skills/i18n-localizer
```

Then open any project and ask Claude to localize it — the skill auto-detects your project type and gets to work.

---

## Problem

Localization projects break down when teams have mixed stacks, inconsistent translation workflows, and no single rollout path.

## Architecture

- Skill-driven workflow that scans codebases, detects framework/i18n context, and routes to the right implementation strategy.
- Supports web and mobile surfaces (Next.js, React, React Native/Expo, SwiftUI) with format-aware translation handling.
- Integrates routing, metadata, and locale file operations in one delivery loop.

## Outcomes

- Faster localization rollout across heterogeneous codebases.
- Standardized i18n implementation patterns instead of one-off scripts.
- Cleaner handoff from technical setup to content translation and QA.


## 🧩 Supported Frameworks

| Framework | Details |
|---|---|
| **Next.js** | App Router & Pages Router |
| **Vite + React** | Fast builds with React |
| **React Router** | v7 |
| **React Native & Expo** | Mobile apps |
| **SwiftUI** | String Catalogs / `xcstrings` |
| **Plain React** | Any React project |

## 📦 Supported Formats

`JSON` · `YAML` · `CSV` · `PO` · `Markdown` · `xcstrings` · `XLIFF`

---

## ✨ What It Does

- 🔍 **Auto-detects** your project type and existing i18n setup
- 📝 **Extracts** hardcoded strings into locale files
- 🤖 **Generates** AI-powered translations for **47+ languages**
- 🔗 **Sets up i18n routing** (`/en/about`, `/es/about`, etc.)
- 🏷️ **Generates** `hreflang` tags and localized SEO metadata
- 🌐 **Handles** pluralization, RTL layout, and date/number formatting
- 🍎 **Supports** Apple String Catalogs for SwiftUI / iOS / macOS apps

---

## 🧠 Strategies

The skill automatically selects the best localization approach for your project:

| Strategy | When to Use |
|---|---|
| **Compiler Approach** ([Lingo.dev](https://github.com/lingodotdev/lingo.dev)) | Zero-runtime i18n, compile-time string replacement |
| **next-intl** | Next.js App Router with server components |
| **react-i18next** | Vite, React Router, or plain React |
| **React Native** | React Native / Expo with i18next |
| **Apple Native** | SwiftUI String Catalogs (`xcstrings`) |
| **Manual Translation** | Direct locale file management |

---

## 🙏 Credits

Built on knowledge from [Lingo.dev](https://github.com/lingodotdev/lingo.dev) (Apache-2.0), Apple Developer documentation, and community best practices.

## 📄 License

This project is licensed under the [MIT License](LICENSE).
