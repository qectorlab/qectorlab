<p align="center">
  <img src="https://raw.githubusercontent.com/GuillaumeLessard/.github/main/profile/logo_banner.png" alt="QECTOR" width="70%" />
</p>

<h2 align="center">Hi, I'm Guillaume Lessard. I build QECTOR.</h2>

<p align="center">
  <strong>Quantum error correction you can check, not just trust.</strong><br/>
  Independent researcher and developer in Longueuil, Québec.
</p>

<p align="center">
  <a href="https://www.qector.store">qector.store</a> ·
  <a href="https://zenodo.org/communities/id01t">Research Archive</a> ·
  <a href="https://orcid.org/0009-0000-3465-3753">ORCID</a> ·
  <a href="https://www.linkedin.com/in/qector">LinkedIn</a> ·
  <a href="https://github.com/GuillaumeLessard">QECTOR organization</a>
</p>

---

### What I work on

I write decoders for quantum error correction codes, and I publish the evidence behind every result. A QECTOR decoder checks its own answer: each correction it returns reproduces the syndrome, **H c = s (mod 2)**, or the call fails.

| Project | What it is |
|:--|:--|
| [**QECTOR Decoder v3**](https://github.com/GuillaumeLessard/qector-decoder) | Python library with a compiled Rust core: Union-Find, exact MWPM, BP-OSD and Relay-BP for qLDPC codes, CPU and GPU batch decoding, Stim and Sinter integration. |
| [**QECTOR Claude Plugin**](https://github.com/GuillaumeLessard/qector-claude-plugin) | Verified QEC decoding inside Claude Code and Claude Desktop, through an air-gapped MCP server. |
| [**QECTOR Decoder Workbench**](https://github.com/qectorlab/qector-decoder-workbench-windows) | Free desktop app for Windows and [Linux](https://github.com/qectorlab/qector-decoder-workbench-linux): explore codes and Tanner graphs, run 19 decoders, export reproducible results. |
| [**qector-proof**](https://github.com/GuillaumeLessard/qector-proof) | Executable certification suite for the decoder, with a hash-locked install. |

```bash
pip install qector-decoder-v3
```

### Recent research

- **[[832, 10, 15]], machine-checked.** A quantum LDPC code with 832 physical qubits, 10 logical qubits and minimum distance exactly 15. Coq proves the whole result with no axioms; Lean and Isabelle cross-check it. [Proofs](https://doi.org/10.5281/zenodo.23956279)
- **Fold-and-lift.** An exact method for certifying the minimum distance of quasi-cyclic CSS codes. For the [[832, 10]] code it takes about one second per sector on one CPU core. [Paper](https://doi.org/10.5281/zenodo.23327681)
- **LCL-832 as a Metastable Effective Theory.** Every theorem of version 4.0 is machine-checked in Coq. [Proofs](https://doi.org/10.5281/zenodo.23956600)

Every record, with the kind of evidence it carries, is in the [QECTOR Research Archive](https://zenodo.org/communities/id01t) on Zenodo.

### Using QECTOR

- **Research and personal use:** QECTOR Decoder v3 is source-available under the PolyForm Noncommercial License 1.0.0, free for personal, academic and non-commercial research.
- **Commercial use:** plans at [qector.store/pricing](https://qector.store/pricing).
- **Bugs and failed reproductions:** open an issue in the repository concerned. For security problems, follow the [security policy](https://github.com/GuillaumeLessard/.github/blob/main/SECURITY.md).
