# Capacity Release Policy (Rev 4)

Applies to standard serving replicas of the Atlas platform.

## Targets

| Metric | Target |
| --- | --- |
| Resident memory | 445 GB |
| Transient memory | 88 GB |

## Verdict scale

Each metric is judged against its own target:

- actual < 95% of target: Under-allocated
- actual > 105% of target: Over-allocated
- otherwise: Within tolerance

## Release decision

- Both metrics Within tolerance: APPROVED
- Otherwise: BLOCKED

## Dossier handling

- Submit the dossier to this repository at audits/RPL-2291/report.md on the default branch.
- For a BLOCKED decision, open an issue in this repository titled exactly
  "[CAPACITY BLOCK] RPL-2291" describing the blocking metrics. No issue is required for
  an APPROVED decision.
