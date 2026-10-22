<div align="center">

# Marcos Gabriel

<sub>**Systems software, from the protocol up.**</sub>

`Rust` · `Python` · `Git internals` · `network protocols` · `databases` · `applied cryptography`

</div>

---

Software Engineering student at **Unifatecie** (Brazil). I learn by rebuilding hard things
from scratch — a version control system, a remote shell, a document database, a remote
desktop. If the interesting part lives inside a dependency, I write the dependency.

### 🦀 Flagship — [cvx](https://github.com/marcosgabrielgomes110-collab/cvx)

**A Git-compatible version control system written in Rust.** It reads and writes real Git
repositories — objects, packs, refs, index, merge — without ever shelling out to `git`.
Git itself stays the test oracle, so compatibility is measured, not claimed.

<p>
<img alt="Rust" src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white">
<img alt="26k lines" src="https://img.shields.io/badge/26k_lines_of_Rust-1f6feb?style=flat-square">
<img alt="21 crates" src="https://img.shields.io/badge/21_crates-1f6feb?style=flat-square">
<img alt="270+ tests" src="https://img.shields.io/badge/270%2B_tests-2ea043?style=flat-square">
<img alt="CI" src="https://img.shields.io/github/actions/workflow/status/marcosgabrielgomes110-collab/cvx/ci.yml?style=flat-square&label=CI">
<img alt="Release" src="https://img.shields.io/github/v/release/marcosgabrielgomes110-collab/cvx?style=flat-square&label=release">
</p>

```console
$ cvx init && cvx add . && cvx commit -m "feat: first commit"
$ cvx switch feature/auth && cvx merge main
$ cvx push origin main          # HTTPS + SSH transport, no git binary involved
```

Built for the boring parts too: SHA-256 repositories, `.gitattributes`/CRLF handling,
property-based fuzzing, crash failpoints and benchmarks.

### The rest of the shelf

| Project | What it does | Under the hood |
|---|---|---|
| **[rmp](https://github.com/marcosgabrielgomes110-collab/rmp)** | SSH-like remote shell built from scratch on QUIC — no `sshd`, no SSH2 | Rust · TLS 1.3 · hybrid **X25519 + ML-KEM-768** |
| **[lunadb](https://github.com/marcosgabrielgomes110-collab/lunadb)** | JSON/MessagePack document database over HTTP: schema validation, encryption at rest, roles/grants, CLI and Python SDK | Rust · Python |
| **[BridgeDesktop](https://github.com/marcosgabrielgomes110-collab/BridgeDesktop)** | Encrypted peer-to-peer remote desktop with no relay servers | Rust · X11 · H.264 · ChaCha20-Poly1305 |
| **[vidra](https://github.com/marcosgabrielgomes110-collab/vidra)** | Fully offline video dubbing pipeline: download, transcribe, translate, synthesize, mux | Python · Vosk · Piper TTS · FFmpeg |
| **[Apex](https://github.com/marcosgabrielgomes110-collab/Apex)** | DAG workflow engine with `@flow` / `@task`, implicit state, zero dependencies | Python · 100+ tests |

### How I ship

- **Green before merge** — CI on Linux, macOS and Windows with `clippy -D warnings`, `rustfmt` and the full test suite.
- **Released, not just pushed** — versioned tags, cross-platform binaries and SHA-256 checksums.
- **Documented like a product** — architecture notes, compatibility specs, security policy and changelog.

### Toolbox

<p>
<img alt="Rust" src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white">
<img alt="Python" src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white">
<img alt="Linux" src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black">
<img alt="Git" src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white">
<img alt="QUIC + TLS" src="https://img.shields.io/badge/QUIC_%2B_TLS_1.3-5C2D91?style=flat-square">
<img alt="MikroTik" src="https://img.shields.io/badge/MikroTik-293239?style=flat-square&logo=mikrotik&logoColor=white">
<img alt="Bash" src="https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white">
<img alt="Windows" src="https://img.shields.io/badge/Windows-0078D6?style=flat-square&logo=windows&logoColor=white">
</p>

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api/top-langs/?username=marcosgabrielgomes110-collab&layout=compact&langs_count=6&hide_title=true&hide_border=true&theme=github_dark">
  <img alt="Most used languages" src="https://github-readme-stats.vercel.app/api/top-langs/?username=marcosgabrielgomes110-collab&layout=compact&langs_count=6&hide_title=true&hide_border=true">
</picture>

<br/>

<sub>🇧🇷 Brazil · always up for a good technical conversation</sub>

</div>
