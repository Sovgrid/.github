<div align="center">

# Sovereign AI Grid

**Open-source tools for running AI on your own hardware: an agent orchestrator, a blog MCP server, and the backup that keeps the box recoverable.**

[**Website**](https://sovgrid.org) · [**Fleet project page**](https://sovgrid.org/fleet/) · [**Upstream work**](https://sovgrid.org/upstream/) · [**Support & Value4Value**](https://sovgrid.org/support/) · [**Nostr**](https://njump.me/cipherfox@sovgrid.org)

</div>

---

### Projects

**[Sovereign Fleet](https://github.com/Sovgrid/sovereign-fleet)** [![release](https://img.shields.io/github/v/release/Sovgrid/sovereign-fleet?style=flat-square&color=06b6d4)](https://github.com/Sovgrid/sovereign-fleet/releases) [![PyPI](https://img.shields.io/pypi/v/sovereign-fleet?style=flat-square&color=06b6d4)](https://pypi.org/project/sovereign-fleet/)
Runs coding-agent CLIs (goose, Aider, OpenCode, Pi, Claude Code) unattended on your own machine: a task queue, a Landlock + seccomp sandbox per run, gates that run the repository's own tests before anything lands, and a router that learns which harness and model pair finishes a kind of task fastest, local models first. Ships goose recipes and an MCP server, so goose can queue and watch fleet tasks. `pip install sovereign-fleet` · [project page](https://sovgrid.org/fleet/)

**[sovereign-mcp](https://github.com/Sovgrid/sovereign-mcp)** [![release](https://img.shields.io/github/v/release/Sovgrid/sovereign-mcp?style=flat-square&color=06b6d4)](https://github.com/Sovgrid/sovereign-mcp/releases)
The MCP server behind [sovgrid.org](https://sovgrid.org): search, list and read the blog's engineering log of self-hosted AI on an NVIDIA DGX Spark, plus a checker for SGLang configs on GB10. Public endpoint, no sign-up: `https://mcp.sovgrid.org/self-hosted-ai` (streamable HTTP). FastMCP, Python 3.12.

**[sovereign-backup](https://github.com/Sovgrid/sovereign-backup)** [![release](https://img.shields.io/github/v/release/Sovgrid/sovereign-backup?style=flat-square&color=06b6d4)](https://github.com/Sovgrid/sovereign-backup/releases)
Config-driven multi-host backup in plain bash: tar plus age encryption to a USB stick or local disk, per-host YAML, a systemd timer, and `restore --verify` to prove a backup opens before you need it.

**[Vozonda](https://github.com/Vozonda/vozonda)** (own organization)
Turns articles, papers, PDFs, videos and feeds into your own podcast on your own hardware: local model, local voices, your own feed, Nostr and Lightning. A self-hosted alternative to NotebookLM's audio overviews.

---

### Principles

* **Kernel confinement:** agents run on the host, confined by the Linux kernel (Landlock ABI 6+ and seccomp), not in a container or VM; they start in milliseconds and still reach the local model server.
* **Verify before claim:** an agent's report is a claim, not proof. The repository's own tests run in a credential-free sandbox before anything merges.
* **Local weights first:** your own model servers (vLLM, SGLang, Ollama) are ranked first; cloud models are lanes you add, not a requirement.
* **Value-for-Value:** independent open-source work, funded by the people who use it, no venture capital.

---

### Nostr

* **Operator:** [`cipherfox@sovgrid.org`](https://njump.me/cipherfox@sovgrid.org): engineering notes and what broke.
* **Releases:** [`blog@sovgrid.org`](https://njump.me/blog@sovgrid.org): release announcements and new articles.

### Support

If the tools are useful to you: Bitcoin Lightning, Nostr zaps or a grant, all on **[sovgrid.org/support](https://sovgrid.org/support/)**.

<div align="center">
<sub>Built for people who run their own AI.</sub>
</div>
