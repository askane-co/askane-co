<div align="center">
  <a href="https://github.com/askane-co/askane">
    <img src="https://raw.githubusercontent.com/askane-co/askane/main/docs/banner.jpg" alt="Askane Banner" width="100%" />
  </a>

  <h1>
    <img src="https://raw.githubusercontent.com/askane-co/askane/main/docs/logo.png" alt="Pleco Logo" width="38" height="38" align="absmiddle" />
    &nbsp;Askane
  </h1>

  <p>
    <strong>Experimental bytecode scripting language written in pure Rust with zero external crates.</strong><br/>
    Designed &amp; built in collaboration with <strong>Gemini</strong> and <strong>ChatGPT</strong>, with full transparency on AI-assisted engineering.
  </p>

  <p>
    <a href="https://github.com/askane-co/askane/releases/latest">
      <img src="https://img.shields.io/github/v/release/askane-co/askane?label=Latest%20Release&color=26b8ec&style=flat-square" alt="Latest Release" />
    </a>
    <a href="https://github.com/askane-co/askane/actions/workflows/ci.yml">
      <img src="https://github.com/askane-co/askane/actions/workflows/ci.yml/badge.svg" alt="CI" />
    </a>
    <a href="https://github.com/askane-co/askane/blob/main/ROADMAP.md">
      <img src="https://img.shields.io/badge/Roadmap-v0.19%E2%80%93v0.22-e97a2e?style=flat-square" alt="Roadmap" />
    </a>
    <img src="https://img.shields.io/badge/Rust-Zero%20Crates-0f172a?style=flat-square" alt="Zero Crates" />
  </p>
</div>

---

### What Makes Askane Different

- **Zero External Dependencies**: Lexer, AST parser, bytecode compiler, register/stack VM (`execute_fast`), AEAD crypto, DEFLATE/ZIP, HTTP/WebSockets, and Win32 Studio IDE all live cleanly in pure Rust stdlib + native OS APIs.
- **Capability-Based Sandbox**: Scripts run default-deny for filesystem access outside root, network (`net`/`ws`/`http`), env/args, clipboard, global input, and subprocesses (`Job Objects`), plus in-language `needs`, `sandbox { ... }`, `with`, and `defer` contracts.
- **49 Built-in Modules & Batteries Included**: `crypto`, `kv` (append-only CRC32 store), `net`, `ws`, cooperative green `task` & `channel`, reactive `signal` (`on change`), declarative 2D `ui` & `gfx`, `json`, `toml`, `csv`, `html`/`xml`, `regex`, `diff`, `log`, and more.
- **Developer Tooling**: Multi-error recovery & structured diagnostics (`E...`/`W...`, `--explain`, `--diagnostic-format=json`, `did you mean`), AST formatter (`fmt`), test runner (`test --deterministic` & snapshots), `doctor`, `info`, `modules`, `clean`, and Askane Studio v2 (`--gui`).

| Metric | Current State (`v0.18.0`) |
| --- | --- |
| External Cargo crates | **0** (`Cargo.toml`) |
| Built-in stdlib modules | **49** |
| Automated unit/integration tests | **59 passing** (`windows-latest` & `ubuntu-latest`) |
| Benchmark score ([`bench/`](https://github.com/askane-co/askane/tree/main/bench)) | **41.35 / 100** (~51% of Python 3.12; targeting **65-75+** in `v0.20.0`) |

---

<div align="center">
  <a href="https://github.com/askane-co/askane">
    <img src="https://raw.githubusercontent.com/askane-co/askane/main/docs/roadmap.jpg" alt="Askane Roadmap" width="100%" />
  </a>
</div>

> **Mascot (Pleco):** Askane's official mascot is **Pleco**, a humble *Plecostomus* armored catfish that cleans up messy code and keeps the tank spotless.
