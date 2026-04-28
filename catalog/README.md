# Aether OnRamp Component Catalog

This directory contains YAML catalog entries that describe the deployable
Aether OnRamp components and the shape of the corresponding `vars/main.yml`
sections.

These files are intended to be consumed by external tooling such as
`aether-ops`. OnRamp itself does not currently load them at runtime.

Each catalog entry can declare:

- Component metadata and documentation links
- Available actions and their Makefile targets
- Dependency relationships between components
- Health probe hints for external consumers
- A JSON-Schema-style description of the component's `vars/main.yml` section

The schema is intentionally focused on field shape and operator-facing
descriptions. Defaults are included only where they are stable across the
shipped configurations.

## Components

The current catalog covers:

- `k8s`
- `5gc`
- `4gc`
- `amp`
- `sdran`
- `oscric`
- `gnbsim`
- `ueransim`
- `oai`
- `srsran`
- `ocudu`
- `n3iwf`
- `cluster`
