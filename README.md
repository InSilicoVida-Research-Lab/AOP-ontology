# Adverse Outcome Pathway Ontology (AOPO)

OBO-aligned ontology starter migrated from the legacy [AOP-KB ontology](../aop-ontology/) using the [Ontology Development Kit (ODK)](https://github.com/INCATools/ontology-development-kit).

## Quick start

```bash
# From a path WITHOUT spaces (ODK requirement):
cd aopo/src/ontology
./run.sh make test
./run.sh make all
```

If your checkout path contains spaces, use Docker directly (see [migration-data/MIGRATION.md](../migration-data/MIGRATION.md)).

## Contents

| Path | Description |
|------|-------------|
| `src/ontology/aopo-edit.owl` | Editor ontology (223 terms from AOP-KB) |
| `src/ontology/aopo-odk.yaml` | ODK project configuration |
| `src/ontology/imports/` | Import modules (RO, IAO, ChEBI, HP) |
| `src/metadata/aopo.yml` | OBO PURL configuration template |

## Migrated term summary

- **93** classes (AOP, KE, MIE, AO, context, modulation, etc.)
- **52** object properties (`has_key_event`, `has_adverse_outcome`, …)
- **3** annotation properties (`PubChemAID`, `PubChemCID`, `UniProtID`)
- **75** named individuals (pathway instances, KERs, MIEs, assay data)

Legacy IRI cross-references: `AOPKB:<term>` on every migrated entity.

See [`../migration-data/aopkb-to-aopo-mapping.csv`](../migration-data/aopkb-to-aopo-mapping.csv) for the complete ID map.

## Regenerate from source

```bash
python3 ../scripts/extract_aop_terms.py
cp ../migration-data/aopo-extracted.owl src/ontology/aopo-edit.owl
```

## License

Apache-2.0 (consistent with the U.S. Federal Government AOP-KB source).
