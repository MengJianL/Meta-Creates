# Meta-Creates 元部门

> "协同可以扁平，治理不能缺位。"

**Meta-Creates** is a **Meta-Department (元部门) architecture framework** — a 13-atom organizational system for autonomous AI agent coordination and governance. It provides a pure-abstract, domain-agnostic, self-evolving infrastructure where `.md` files define agent behaviors, and the structure itself is the product.

## What is a Meta-Department?

A Meta-Department is an organizational pattern inspired by real-world corporate structures, applied to AI agent systems. Instead of monolithic prompts or ad-hoc agent chains, Meta-Creates decomposes agent coordination into **13 irreducible atomic units** ("atoms") arranged in a three-layer gravity structure — mirroring how real organizations separate infrastructure, management, and execution.

The key insight: **governance cannot be absent**. Just as a company needs clear roles, communication channels, and quality oversight, an AI agent system needs the same — formalized, self-evolving, and domain-agnostic.

## Architecture: Three-Layer Gravity Structure

```
┌─────────────────────────────────────────────────────────────────────┐
│  Layer 3 — Execution (原子操作)                                      │
│  M09-compose(写)   M10-retrieve(查)  M11-invoke(用)                  │
│  M12-verify(检)    M13-create(创)                                    │
├─────────────────────────────────────────────────────────────────────┤
│  Layer 2 — Orchestration (编排协调) [Critical & Deep Thinking]       │
│  M04-decompose  M05-route  M06-evaluate  M07-synthesize  M08-sequence│
├─────────────────────────────────────────────────────────────────────┤
│  Layer 1 — Foundation (基础设施)                                      │
│  M01-memory        M02-identity        M03-channel                   │
└─────────────────────────────────────────────────────────────────────┘
```

| Layer | Atoms | Role |
|-------|-------|------|
| **Foundation** | M01 Memory · M02 Identity · M03 Channel | Storage, identity, and communication infrastructure |
| **Orchestration** | M04 Decompose · M05 Route · M06 Evaluate · M07 Synthesize · M08 Sequence | Coordinate, route, evaluate, and sequence — all with Critical & Deep Thinking |
| **Execution** | M09 Compose · M10 Retrieve · M11 Invoke · M12 Verify · M13 Create | Atomic operations: compose, query, invoke, verify, create |

## The 13 Atoms

| # | Atom | Op | Core Responsibility |
|---|------|----|---------------------|
| M01 | Memory 记忆元 | — | Layered storage, compression, and isolated retrieval |
| M02 | Identity 身份元 | — | Role boundaries, behavioral constraints, capability profiles |
| M03 | Channel 通信元 | — | Inter-layer information flow control and filtering |
| M04 | Decompose 分解元 | — | Intent decomposition and Intent Amplification Ratio (IAR) |
| M05 | Route 路由元 | — | Capability-matched routing + skill discovery |
| M06 | Evaluate 评估元 | — | Multi-dimensional independent quality assessment |
| M07 | Synthesize 聚合元 | — | Multi-source deduplication, integration, conflict detection |
| M08 | Sequence 序列元 | — | Pipeline orchestration and stage gating |
| M09 | Compose 构成元 | 写 | Compose candidate content objects under constraints |
| M10 | Retrieve 检索元 | 查 | Locate and extract contextually relevant information |
| M11 | Invoke 调用元 | 用 | Trigger external tools/APIs and process results |
| M12 | Verify 验证元 | 检 | Constraint-set verification and gate decisions |
| M13 | Create 创造元 | 创 | Pattern recombination, skill engineering, agent creation |

## Five Core Questions

The 13 atoms are not 13 parallel actions — they form a complete structure from **continuous existence → organized progression → independent governance → result formation → capability extension**:

1. **How does the system persist?** — M01 / M02 / M03
2. **How does the system organize problems?** — M04 / M05 / M08
3. **How does the system judge quality and validity?** — M06 / M12
4. **How does the system produce and advance results?** — M09 / M10 / M11 / M07
5. **How does the system extend its own capabilities?** — M13

## Five Core Chains

```
Chain 1 (Standard Task):     M03 → M04 → M05 → M08 → M09/M10/M11 → M12 → M06 → M07 → M03
Chain 2 (Candidate Generation): M04 → M05 → M09 → M12 → M06 → M07
Chain 3 (Retrieval & Reuse):    M04/M05 → M10 → M12/M06 → M07
Chain 4 (External Capability):  M05 → M11 → M12 → M06 → M07
Chain 5 (Capability Creation):  M05/M10/M01 → M13 → M12 → M06 → M01 → M05
```

## Two Governance Loops

- **Quality Loop**: Execution output → M12 verify → M06 evaluate → reflow to origin → re-execute
- **Evolution Loop**: Historical gaps → M13 create → M12 verify → M06 evaluate → M01 persist → M05 route for reuse

## M06 vs M12: Evaluate vs Verify

A critical architectural distinction:

| | M06 Evaluate | M12 Verify |
|---|---|---|
| **Question** | "Is it good enough?" | "Does it hold up?" |
| **Judges** | Quality, completeness, actionability | Validity, consistency, constraint satisfaction |
| **Output** | Score + pass/fail + improvement direction | Pass/fail per condition + failure points |

## Design Principles

1. **Irreducibility** — Each atom, if further decomposed, loses independent semantic integrity
2. **Pure Abstraction** — No domain-specific vocabulary; cross-domain reusable
3. **Self-Evolution** — Every atom has built-in feedback-driven adaptation
4. **Orthogonality** — Clear boundaries, no functional overlap
5. **Governance First** — Each atom answers: what am I, what am I not, how am I governed, how do I evolve
6. **Evolvable Architecture** — M13 has five creation levels: Project Agents (L0), Skills (L1), Agents (L2), Meta-Departments (L3), and Governance-Aware Replication (L4)

## Project Agent System

The Meta-Department is a **"tool that creates tools"** (创造工具的工具). Its primary output is **Project Agent definitions** — standardized `.md` files stored in the project's `agents/` directory — not work deliverables. The department creates tools, then uses those tools to do work.

### Three-Layer Tool Hierarchy

```
┌─────────────────────────────────────────────────┐
│  Project Agent Definitions                        │  ← Tools created by Meta-Department
│  Stored in agents/, reusable, iterable, cumulative │
├─────────────────────────────────────────────────┤
│  13 Atoms (.claude/agents/)                       │  ← Infrastructure for creating Agents
│  Abstract role templates, not direct executors     │
├─────────────────────────────────────────────────┤
│  Claude Code Agent Tool                           │  ← Runtime execution mechanism
│  Ephemeral subprocess, executes per Agent def      │
└─────────────────────────────────────────────────┘
```

### Triple-Armed Agent Definitions

Each Project Agent is **triple-armed** (Prompt + Skill + Tools) with a **9-section template**:

1. **Identity** — Role positioning, domain expertise, decision authority
2. **Atom Mapping** — Which M## atom(s) it instantiates
3. **Input Contract** — Accepted formats, validation rules, prerequisites
4. **Output Contract** — Normal output, failure reports, downstream receivers
5. **Execution Protocol** — Imperative step-by-step procedure
6. **Behavioral Constraints** — Must-do, must-not-do, context isolation
7. **Quality Standards** — Quantified acceptance criteria, verification method
8. **Skill Loadout** — Core and auxiliary skills (auto-matched from atom affinity tables)
9. **Tool Priority** — Primary, auxiliary, and forbidden tools (auto-matched from atom tables)

### Reuse-Before-Create Principle

When routing tasks, M05 follows this priority chain:

1. **Match in `agents/`** → Reuse existing Project Agent definition
2. **Match in global resources** (`.claude/skills/`, `.claude/agents/`, `references/`) → Invoke directly via Skill tool
3. **No match** → Create new Project Agent definition → Verify → Then execute
4. **Partial match** → Update Agent definition version, record changes

## M13: Five-Level Creation

M13 (Create) has **five-level creation capabilities** (L0–L4):

| Level | What | Storage | Gate |
|-------|------|---------|------|
| **L0: Project Agent** | Project-specific Agent definitions (most common) | `agents/` | No gate — standard Meta-Department output |
| **L1: Skill** | Reusable patterns & modules | Internal | 2x validation + clear I/O contract |
| **L2: Agent** | New atomic units with identity & evolution | `.claude/agents/` | 5-gate process (gap → skill insufficient → layer → orthogonality → human confirm) |
| **L3: Meta-Department** | Full 13-atom system instances | Independent directory | Lineage tracking + governance sync + independent evolution |
| **L4: Governance-Aware Replication** | Parent-child Meta-Department replication with version, inheritance, diff control, and governance synchronization | Independent directory | Not arbitrary replication — structurally governed expansion |

L0 (Project Agent) is the most frequent creation act — on every task, the Meta-Department first creates or reuses Agent definitions in `agents/`, then dispatches execution according to those definitions. This embodies the core philosophy of "a tool that creates tools."

### Architecture Safety Valves

- **Atom count limit**: When total atoms exceed 18, an architecture review is triggered.
- **M13 halt rules**: M13 includes a complete stop-rule system — creation at each level has explicit halt conditions to prevent runaway self-replication. Level escalation (e.g., L1→L2) requires demonstrating that the lower level is insufficient, not merely inconvenient.

## Usage: The `/meta` Command

The primary entry point for the Meta-Department is the **`/meta <task>`** slash command (defined in `.claude/commands/meta.md`). It orchestrates the full pipeline:

1. **Intent Amplification** — Fuzzy tasks are expanded along three dimensions for user selection
2. **Analysis** — Task decomposition (M04) and routing design (M05)
3. **Agent Creation/Reuse** — Check `agents/` for existing definitions; create new ones if needed
4. **Execution** — Dispatch Agents according to their definitions
5. **Verification & Evaluation** — Independent M12 verify and M06 evaluate (separation of powers)
6. **Delivery** — Synthesize results and deliver

Hard gate-checks are enforced between phases. Standard/heavy tasks cannot enter execution without first completing Agent definition creation/reuse.

## Cross-Project Reuse

To bootstrap a new project with the Meta-Department framework:

```bash
# Copy the 13 atoms + architecture index
cp -r .claude/agents/ your-project/.claude/agents/

# Do NOT copy agents/ — Project Agent definitions are project-specific
# Do NOT copy .claude/memory/ — each project accumulates its own memory (M01 principle)
```

## Project Structure

```
Meta-Creates/
├── agents/                    # Project Agent definitions (created by Meta-Department)
├── .claude/
│   ├── agents/                # 13 atoms + architecture index
│   │   ├── CLAUDE.md          # Architecture index (总纲)
│   │   ├── M01-memory.md      # Foundation: Memory
│   │   ├── M02-identity.md    # Foundation: Identity
│   │   ├── M03-channel.md     # Foundation: Channel
│   │   ├── M04-decompose.md   # Orchestration: Decompose
│   │   ├── M05-route.md       # Orchestration: Route
│   │   ├── M06-evaluate.md    # Orchestration: Evaluate
│   │   ├── M07-synthesize.md  # Orchestration: Synthesize
│   │   ├── M08-sequence.md    # Orchestration: Sequence
│   │   ├── M09-compose.md     # Execution: Compose (写)
│   │   ├── M10-retrieve.md    # Execution: Retrieve (查)
│   │   ├── M11-invoke.md      # Execution: Invoke (用)
│   │   ├── M12-verify.md      # Execution: Verify (检)
│   │   └── M13-create.md      # Execution: Create (创)
│   └── commands/
│       └── meta.md            # /meta slash command
├── references/                    # Papers, prompt libraries, skill playbooks
│   └── base/                      # Source paper + architecture diagrams
├── CLAUDE.md                      # Project instructions for Claude Code
└── README.md
```

## Contributors

- **[MengJianL](https://github.com/MengJianL)** — Architecture design, atom specifications, governance framework
- **[Claude](https://claude.ai)** (Anthropic) — Architecture co-design, documentation, implementation
- **[ChatGPT](https://chatgpt.com)** (OpenAI) — Architecture co-design, documentation, implementation

## Acknowledgments

Special thanks to **[KimYx0207](https://github.com/KimYx0207)** for invaluable contributions and support throughout the development of this project.

## References

> 孟健, 金仲旭. *基于"组织镜像"理论的AI智能体多Agent协作架构设计*. Zenodo, 2025.
>
> Meng Jian, Jin Zhongxu. *AI Agent Multi-Agent Collaboration Architecture Design Based on "Organizational Mirroring" Theory*. Zenodo, 2025.

- **DOI**: [https://zenodo.org/records/18957649](https://zenodo.org/records/18957649)

## License

MIT
