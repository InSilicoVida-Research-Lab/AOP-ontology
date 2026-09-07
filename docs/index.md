# Adverse Outcome Pathway Ontology (AOPO)

An OBO-aligned ontology for adverse outcome pathways (AOPs) in computational toxicology.

## Quick start

```bash
# From a path WITHOUT spaces (ODK requirement):
cd src/ontology
./run.sh make test
./run.sh make all
```

If your checkout path contains spaces, use Docker directly (see the repository README).

## Repository layout

| Path | Description |
|------|-------------|
| `src/ontology/aopo-edit.owl` | Editor ontology |
| `src/ontology/aopo-odk.yaml` | ODK project configuration |
| `src/ontology/imports/` | Import modules (RO, IAO, ChEBI, HP) |
| `src/metadata/aopo.yml` | OBO PURL configuration template |

## Links

- [GitHub repository](https://github.com/InSilicoVida-Research-Lab/AOP-ontology)
- [Issue tracker](https://github.com/InSilicoVida-Research-Lab/AOP-ontology/issues)
- [OBO Foundry PURL](http://purl.obolibrary.org/obo/aopo.owl)

## License

Licensed under [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0).
