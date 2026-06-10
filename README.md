# Hi, I'm Tobi Adesoye 👋

### Systems Architect & AI Infrastructure Engineer
I build hardware-aware optimization layers, deterministic execution frameworks, and low-level tensor routing middleware for distributed deep learning loops.

---

## ⚡ Current Main Focus: `renorm-native`
I am the author of **[renorm-native](https://github.com/Tobi-Adesoye/renorm-native)**, a completely decoupled, self-bootstrapping middleware layer that eliminates cumulative memory fragmentation and delayed CUDA/ROCm OOM cliffs in long-context transformer architectures. 

* **Zero-Dependency Hook:** Acts as a passive layout referee via an externalized profile matrix (`gateway_profiles.json`).
* **Register-Fused Optimization:** Bypasses off-chip HBM round-trips by locking dynamic tensor structures inside local SRAM registers via Triton.

---

## 🔬 Core Technical Analysis & Research
If you are managing multi-node accelerator clusters or fighting unhandled allocation crashes mid-run, check out my definitive engineering guide on memory physics:

### 📑 [Read: Why Your PyTorch Models Crash at Step 200: The Physics of Cumulative Memory Fragmentation]https://medium.com/@adesoyetobe/why-your-pytorch-models-crash-at-step-200-the-physics-of-cumulative-memory-fragmentation-0b2fc37cd92c?postPublishedType=repub
*An in-depth micro-architectural deep-dive exploring how uncoalesced memory transit steps leave jagged micro-gaps across physical cache lines, why standard caching allocators panic, and how block-level tensor padding stabilizes the VRAM floor permanently.*

---

## 🛠️ Expertise & Domain Focus
* **Hardware Architecture:** NVIDIA HBM3e layout mapping, AMD ROCm/wave64 sector alignment.
* **Framework Runtimes:** Deep PyTorch internals, custom Triton kernels, vLLM worker clustering, FSDP tensor sharding.
* **System Design:** Property-driven declarative metadata engines, zero-maintenance middleware.

📫 **Let's stabilize your compute:** If your infrastructure team is scaling high-throughput serving architectures, enterprise SFT runs, or complex agent loops and hitting memory ceilings, open an issue on `renorm-native` or reach out for custom cluster profiling.
