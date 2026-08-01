# nauti-inferer

Public **inference engine** product (GPU serve, kernels, model load path).

> **Monorepo note:** Today the engine crate lives at `wreckhunter2000-1/core/cesarops-inference/` while `backend/nauti-inferer/` is the distributed control plane. On extract, engine code maps **here**; the distributed program maps to [`cesarops-inference`](https://github.com/festeraeb/cesarops-inference). Desktop client remains [`nauti-inferer-client`](https://github.com/festeraeb/nauti-inferer-client).

## Intended contents

| Monorepo path | Role |
|---|---|
| `core/cesarops-inference/` | Native Rust LLM engine |
| Engine-only scripts / systemd unit fragments | Deploy helpers |

**Out of scope:** GGUF/safetensors weights, fleet scheduler, Forge.
