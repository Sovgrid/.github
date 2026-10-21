<div align="center">

# Sovereign AI Grid

**Open-source software, kernel-sandboxed agent orchestrators, and sovereign computing stacks for local hardware.**

[**Website**](https://sovgrid.org) · [**Fleet Project Page**](https://sovgrid.org/fleet/) · [**Support & Value4Value**](https://sovgrid.org/support/) · [**Nostr**](https://njump.me/cipherfox@sovgrid.org)

</div>

---

### Core Projects

* **[Sovereign Fleet](https://github.com/Sovgrid/sovereign-fleet)** (`sovereign-fleet`):
  Kernel-sandboxed task queue, Thompson-sampling `(harness × model)` router, deterministic quality gates, and mobile-first control plane for autonomous coding-agent CLIs (Goose, Aider, Claude Code, OpenCode, Pi). Zero cloud dependencies, Linux Landlock LSM + seccomp confinement.

* **[Vozonda](https://github.com/Vozonda/vozonda)**:
  Turn sources into your podcast. Open-source, self-hosted alternative to NotebookLM audio overviews: your own RSS feed, local models, Nostr and Lightning.

* **[Sovereign MCP](https://github.com/cipherfoxie/sovereign-mcp)**:
  Model Context Protocol servers for the Sovereign AI stack (diagnostic, knowledge-base search, and inference tools).

---

### Architecture & Principles

* **Kernel Confinement:** Agents run directly on host or VM, confined at the syscall level by the Linux kernel (Landlock ABI 6+ and seccomp). No heavy container overhead.
* **Verify Before Claim:** An agent's execution is a claim, not proof. Independent compilation and test gates must pass inside a credential-free sandbox before anything merges.
* **Local Weights First:** Thompson sampling ranks models and harnesses on your own hardware first (vLLM, SGLang, Ollama) before falling back to external tiers.
* **Value-for-Value:** Independent open-source development funded directly by operators without venture capital.

---

### Connect on Nostr

* **Operator:** [`cipherfox@sovgrid.org`](https://njump.me/cipherfox@sovgrid.org) (engineering war stories, technical observations)
* **Grid Releases:** [`@sovgrid`](https://njump.me/blog@sovgrid.org) (official release announcements and changelog dispatches)

---

### Support & Sponsoring

We believe in **Value-for-Value**. If you find our tools useful, consider supporting open-source development via Bitcoin Lightning, Nostr zaps, or grants:

👉 **[Support Sovereign AI Grid on sovgrid.org/support](https://sovgrid.org/support/)**

---

<div align="center">
<sub>Built for sovereign hackers and local-first AI builders.</sub>
</div>
