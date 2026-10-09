# phosphene

## Rust systems engineer building verifiable infrastructure for autonomous systems

I build systems that make agent-driven changes **constrained, auditable, and testable**.

My work focuses on the boundary where software agents affect real state:

- state-transition and outcome verification;
- constrained NixOS configuration changes;
- evidence-preserving data and security workflows;
- reproducible Rust systems tooling.

I do not treat a model's explanation as proof. The useful question is: **what was allowed, what changed, and what evidence supports the result?**

## Start here

### [`v9r`](https://github.com/ph0xphene/v9r) — verification flagship

Research on state-transition verification with measured trust and observer boundaries. The repository distinguishes supported evidence from stronger guarantees it cannot establish.

**Status:** research software. The [public reviewer entrypoint](https://github.com/ph0xphene/v9r) documents its research and observer boundaries. A separate local transactional-runtime candidate is being prepared; it is not yet a published release.

### [`nix-agent`](https://github.com/ph0xphene/nix-agent) — constrained execution primitive

A local tool that turns natural-language requests into isolated NixOS modules. It separates planning, validation, review, and privileged application rather than giving a model arbitrary shell access.

**Status:** experimental alpha. Its [README](https://github.com/ph0xphene/nix-agent#status) describes review, privilege, and rollback limitations.

### [`sentinel-warehouse`](https://github.com/ph0xphene/sentinel-warehouse) — evidence and state-integrity research

A Python research platform that ingests source data, reconstructs deterministic financial state, checks explicit invariants, and preserves incidents and provenance for replay.

**Status:** research platform, not production financial infrastructure.

## Portfolio thesis

```text
intent
  -> constrained plan
  -> explicit review boundary
  -> action
  -> observed state transition
  -> evidence-backed outcome
```

The repositories are separate experiments, not a single product. Their shared engineering question is how to make consequential automation easier to constrain, inspect, and verify.

## Evidence and limits

- Local verification of `v9r` and `nix-agent` exercises Rust tests and strict lint checks; new CI definitions are prepared but their hosted runs are not yet public evidence.
- `sentinel-warehouse` has deterministic unit coverage plus a separate PostgreSQL integration path.
- These projects are research and alpha software. They do not provide universal sandboxing, arbitrary program verification, or a guarantee that unobserved external effects did not occur.
- Experimental projects such as [`astral`](https://github.com/ph0xphene/astral), [`zkwire`](https://github.com/ph0xphene/zkwire), and [`wired-transport`](https://github.com/ph0xphene/wired-transport) remain secondary laboratory work.

## Selected areas

`Rust` · `Linux` · `NixOS` · `state machines` · `verification` · `provenance` · `security tooling` · `reproducible systems`

For collaboration or focused technical feedback, open an issue in the relevant repository.
