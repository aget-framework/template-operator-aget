# Template: Operator Agent

> Maintain system health with incident handling and operational playbooks

**Version**: v3.5.0 | **Archetype**: Operator | **Skills**: 2 specialized + 13 universal

---

## Why Operator?

The Operator archetype ensures **operational reliability** for systems and services. Unlike development-focused agents, operator agents specialize in:

- **Incident response** — Handle issues with structured triage, investigation, and resolution
- **Playbook execution** — Run standard operating procedures with tracking and verification
- **System health** — Maintain operational continuity through proactive monitoring

**For evaluators**: If you need an AI that can handle incidents methodically and execute operational procedures reliably, the Operator archetype brings SRE discipline to your workflow.

---

## Skills

Operator agents come with **2 archetype-specific skills** plus 13 universal AGET skills.

### Archetype Skills

| Skill | Description |
|-------|-------------|
| **aget-handle-incident** | Handle incidents with structured triage, impact assessment, and resolution tracking. Documents timeline and actions. |
| **aget-run-playbook** | Execute operational playbooks with step verification and rollback options. Tracks completion and exceptions. |

### Universal Skills

All AGET agents include session management, knowledge capture, and health monitoring:

- `aget-wake-up` / `aget-wind-down` — Session lifecycle
- `aget-create-project` / `aget-review-project` — Project management
- `aget-record-lesson` / `aget-capture-observation` — Learning capture
- `aget-check-health` / `aget-check-kb` / `aget-check-evolution` — Health monitoring
- `aget-propose-skill` / `aget-create-skill` — Skill development
- `aget-save-state` / `aget-file-issue` — State and issue management

---

## Ontology

Operator agents use a **formal vocabulary** of 7 concepts organized into 2 clusters:

| Cluster | Concepts |
|---------|----------|
| **Incident Management** | Incident, Severity, Resolution, Timeline |
| **Operations** | Playbook, Step, Runbook |

This vocabulary enables precise communication about operational activities.

See: [`ontology/ONTOLOGY_operator.yaml`](ontology/ONTOLOGY_operator.yaml)

---

## Quick Start

```bash
# 1. Clone the template
git clone https://github.com/aget-framework/template-operator-aget.git my-operator-agent
cd my-operator-agent

# 2. Configure identity
# Edit .aget/version.json:
#   "agent_name": "my-operator-agent"
#   "domain": "your-domain"

# 3. Verify setup
python3 -m pytest tests/ -v
# Expected: All tests passing
```

### Try the Skills

```bash
# In Claude Code CLI
/aget-handle-incident   # Respond to an incident
/aget-run-playbook      # Execute operational procedure
```

---

## What Makes Operator Different

| Aspect | Ad-hoc Response | Operator Agent |
|--------|----------------|----------------|
| **Incidents** | Reactive chaos | Structured triage and resolution |
| **Procedures** | Manual steps | Verified playbook execution |
| **Documentation** | Post-hoc | Real-time timeline |
| **Rollback** | Improvised | Planned reversion paths |

---

## Framework Specification

| Attribute | Value |
|-----------|-------|
| **Framework** | [AGET v3.5.0](https://github.com/aget-framework/aget) |
| **Archetype** | Operator |
| **Skills** | 15 total (2 archetype + 13 universal) |
| **Ontology** | 7 concepts, 2 clusters |
| **License** | Apache 2.0 |

---

## Learn More

- **[AGET Framework](https://github.com/aget-framework/aget)** — Core framework documentation
- **[Archetype Guide](https://github.com/aget-framework/aget/blob/main/docs/ARCHETYPE_GUIDE.md)** — All 12 archetypes explained
- **[Getting Started](https://github.com/aget-framework/aget/blob/main/docs/GETTING_STARTED.md)** — Full onboarding guide

---

## Related Archetypes

| Archetype | Best For |
|-----------|----------|
| **[Worker](https://github.com/aget-framework/template-worker-aget)** | Task execution |
| **[Developer](https://github.com/aget-framework/template-developer-aget)** | Code and build processes |
| **[Supervisor](https://github.com/aget-framework/template-supervisor-aget)** | Fleet coordination |

---

**AGET Framework** | Apache 2.0 | [Issues](https://github.com/aget-framework/template-operator-aget/issues)
