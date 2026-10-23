# Marcos Gabriel

Systems software in Rust and Python. I build the layer under the library call.

Most of what I write starts with a format or a protocol I would rather not take on
faith — Git's object store, a PTY over QUIC, records encrypted at rest. Reading the
spec is usually cheaper than debugging an abstraction over it. When the interesting
part lives inside a dependency, I write the dependency.

Software Engineering at Unifatecie, Brazil.

## Work

**[cvx](https://github.com/marcosgabrielgomes110-collab/cvx)** — Git-compatible version
control system, written in Rust. It reads and writes real repositories: loose objects,
delta packs, refs, the index, merges, SHA-256 repositories. It never shells out to `git`;
upstream `git` stays in the test suite as the oracle, so compatibility is measured
instead of claimed.

- **[rmp](https://github.com/marcosgabrielgomes110-collab/rmp)** — remote shell built on
  QUIC and TLS 1.3, with hybrid X25519 + ML-KEM-768 key exchange and a PTY over streams.
  No `sshd`, no SSH2, no tunneling.
- **[lunadb](https://github.com/marcosgabrielgomes110-collab/lunadb)** — document database
  over HTTP: JSON/MessagePack records, optional schema validation, fields encrypted at
  rest, roles and hashed API keys, dependency-free Python SDK. Pre-1.0, so the on-disk
  format will move.
- **[BridgeDesktop](https://github.com/marcosgabrielgomes110-collab/BridgeDesktop)** —
  peer-to-peer remote desktop: X11 SHM or DXGI capture, H.264, UDP with
  ChaCha20-Poly1305, XOR parity to recover a lost fragment. No relay in the middle.
- **[vidra](https://github.com/marcosgabrielgomes110-collab/vidra)** — offline dubbing
  pipeline: fetch, transcribe with Vosk, translate, synthesize with Piper, mux with FFmpeg.
  Nothing leaves the machine.
- **[Apex](https://github.com/marcosgabrielgomes110-collab/Apex)** — zero-dependency DAG
  workflow engine. `@flow` and `@task` decorators, state inferred from the source, small
  enough to finish in one sitting.

## How I work

- Compatibility is a test result, not a claim: the reference tool runs in CI next to mine.
- Rust CI gates on `clippy -D warnings` and `rustfmt`, then the full suite on Linux, macOS
  and Windows.
- Released means tagged — versioned tags, cross-platform binaries, checksums, changelog.

## Toolbox

`Rust` · `Python` · `Linux` · `Git internals` · `QUIC + TLS 1.3` · `applied cryptography`

Open to technical conversations — the issues tab on any repository is the fastest way
to reach me.
