# TechCorp Backstage Catalog

This repository contains the catalog entities for TechCorp's Backstage developer portal.

## Structure

```
catalog/
├── all.yaml              # Root location file (Backstage entry point)
├── domains/              # Business domain definitions
├── systems/              # System definitions
├── components/           # Service/component definitions
├── resources/            # Infrastructure resource definitions
└── templates/            # Golden path templates
```

## Usage

This repository is automatically read by Backstage using the GitHub integration.
Changes pushed to this repo will be discovered by Backstage within a few minutes.

## Adding New Entities

1. Create YAML files in the appropriate subdirectory
2. Add a reference to the new file in `catalog/all.yaml`
3. Push changes to GitHub
4. Wait for Backstage to discover the new entities (usually 1-5 minutes)
