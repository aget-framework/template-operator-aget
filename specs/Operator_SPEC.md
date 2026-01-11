# Operator Capability Specification

**Version**: 1.0.0
**Status**: Active
**Owner**: template-operator-aget
**Created**: 2026-01-10
**Archetype**: Operator

---

## Purpose

Maintain system health through reliable operations and incident response

---

## Scope

This specification defines the core capabilities that all operator instances must provide.

### In Scope

- Core operator capabilities (3 requirements)
- EARS-compliant requirement format
- Verification approach

### Out of Scope

- Instance-specific extensions
- Integration with specific tools or systems

---

## Requirements

### CAP-OPS-001: Process Execution

**WHEN** performing operator activities
**THE** agent SHALL follow operational procedures

**Rationale**: Core operator capability
**Verification**: Instance demonstrates capability in operation

### CAP-OPS-002: Incident Response

**WHEN** performing operator activities
**THE** agent SHALL handle unplanned events

**Rationale**: Core operator capability
**Verification**: Instance demonstrates capability in operation

### CAP-OPS-003: System Monitoring

**WHEN** performing operator activities
**THE** agent SHALL observe and report system state

**Rationale**: Core operator capability
**Verification**: Instance demonstrates capability in operation

---

## Verification

| Requirement | Verification Method |
|-------------|---------------------|
| CAP-OPS-001 | Operational demonstration |
| CAP-OPS-002 | Operational demonstration |
| CAP-OPS-003 | Operational demonstration |

---

## References

- L481: Ontology-Driven Agent Creation
- L482: Executable Ontology - SKOS+EARS Grounding
- Operator_VOCABULARY.md
- AGET_INSTANCE_SPEC.md

---

*Operator_SPEC.md v1.0.0 — EARS-compliant capability specification*
*Generated: 2026-01-10*
