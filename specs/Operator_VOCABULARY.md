# Operator Domain Vocabulary

**Version**: 1.0.0
**Status**: Active
**Owner**: template-operator-aget
**Created**: 2026-01-10
**Scope**: Template vocabulary (DRIVES instance behavior per L481)
**Archetype**: Operator

---

## Meta

```yaml
vocabulary:
  meta:
    domain: "operations"
    version: "1.0.0"
    owner: "template-operator-aget"
    created: "2026-01-10"
    theoretical_basis:
      - "L481: Ontology-Driven Agent Creation"
      - "L482: Executable Ontology - SKOS+EARS Grounding"
    archetype: "Operator"
```

---

## Concept Scheme

```yaml
Operator_Vocabulary:
  skos:prefLabel: "Operator Vocabulary"
  skos:definition: "Vocabulary for operator domain agents"
  skos:hasTopConcept:
    - Operator_Core_Concepts
  rdf:type: skos:ConceptScheme
```

---

## Core Concepts

### Process

```yaml
Process:
  skos:prefLabel: "Process"
  skos:definition: "Repeatable sequence of activities"
  skos:broader: Operator_Core_Concepts
  skos:inScheme: Operator_Vocabulary
```

### Incident

```yaml
Incident:
  skos:prefLabel: "Incident"
  skos:definition: "Unplanned event requiring response"
  skos:broader: Operator_Core_Concepts
  skos:inScheme: Operator_Vocabulary
```

### Runbook

```yaml
Runbook:
  skos:prefLabel: "Runbook"
  skos:definition: "Documented procedure for operations"
  skos:broader: Operator_Core_Concepts
  skos:inScheme: Operator_Vocabulary
```

### Monitoring

```yaml
Monitoring:
  skos:prefLabel: "Monitoring"
  skos:definition: "Continuous observation of system state"
  skos:broader: Operator_Core_Concepts
  skos:inScheme: Operator_Vocabulary
```

### Recovery

```yaml
Recovery:
  skos:prefLabel: "Recovery"
  skos:definition: "Restoration of normal operations after incident"
  skos:broader: Operator_Core_Concepts
  skos:inScheme: Operator_Vocabulary
```

---

## Extension Points

Instances extending this template vocabulary should:
1. Add domain-specific terms under appropriate broader concepts
2. Maintain SKOS compliance (prefLabel, definition, broader/narrower)
3. Reference foundation L-docs where applicable
4. Use `research_status` for terms under investigation

---

## References

- L481: Ontology-Driven Agent Creation
- L482: Executable Ontology - SKOS+EARS Grounding
- R-REL-015: Template Ontology Conformance
- AGET_VOCABULARY_SPEC.md

---

*Operator_VOCABULARY.md v1.0.0 — SKOS-compliant template vocabulary*
*Generated: 2026-01-10*
