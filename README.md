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



## License

