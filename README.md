# dea-catalog-blueprints

> DEA catalog for **Blueprint** — OpenDEAM v0.4.0 (ADR-0004; renamed from `dea-catalog-reference-models`).

## Blueprint (`BLU`)

- **Entity id:** `dea:entity-blueprint`
- **Allocation:** L2 · L2-reusable-knowledge
- **Status:** planned

A composed, reusable target-state design assembled from Architecture Patterns,
providing a template for solution design. Renamed from **Reference Model** in
v0.4.0 (ADR-0004 D5).

## Relationships (from the OpenDEAM model)

- **BLU → AP** — composed of (composition, 1:1..N)

## Allocation contract

This repo's `metamodel-pointer.yaml` is validated in CI against the pinned
OpenDEAM root model (`v0.4.0`) via the reusable
`validate-against-model.yml` workflow. Drift fails CI.

Content (entity instances) lands when the entity promotes from
`planned` to `scaffold` per the model lifecycle.

## License

Apache 2.0 — see [LICENSE](./LICENSE) and [NOTICE](./NOTICE).
