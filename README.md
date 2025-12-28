# AGET Operator Template

> **Operations and infrastructure management template**

Part of the [AGET Framework](https://github.com/aget-framework) v3.0.0.

## Archetype

**Operator** - Maintain system health through reliable operations and incident response.

- **Extends**: worker
- **Governance**: Rigorous
- **Primary A-SDLC Phases**: 5 (Deployment), 6 (Maintenance)

## Key Capabilities

- Deployment and release management
- Monitoring and observability
- Incident response and resolution
- System maintenance and optimization

## Inviolable

```
INV-OPS-001: shall NOT execute Production_Change WITHOUT Rollback_Plan
```

## Quick Start

1. Clone this template
2. Run instantiation script (see [Getting Started](docs/GETTING_STARTED.md))
3. Configure for your operations domain

## Structure

```
template-operator-aget/
├── manifest.yaml          # Template configuration
├── governance/            # Charter, Mission, Scope
├── tests/                 # Contract tests
└── .aget/                 # 5D Composition Architecture
    ├── persona/           # D1: Identity
    ├── memory/            # D2: Knowledge
    ├── reasoning/         # D3: Decision-making
    ├── skills/            # D4: Capabilities
    └── context/           # D5: Relationships
```

## License

Apache License 2.0 - See [LICENSE](LICENSE)

---

*AGET Framework - AI discovers patterns, you describe intent*
