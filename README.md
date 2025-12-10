# Fairground Dataset Cache 🗃️

This repository contains a cache of all datasets from the Fairground project whose licenses allow for redistribution.

For additional context, please refer to the main repository: https://github.com/reliable-ai/fairground

## Generate Cache

The datasets are exported using the fairml-datasets CLI tool. To generate / update the cache, run the following commands:

````bash
# Export datasets using CLI
uvx fairml-datasets@latest export-datasets --collection=PermissivelyLicensedFull --stage=loaded --format=parquet --output-path=./fairground_cache --include-large-datasets

# Compress the cache directory for convenient download / sharing
zip -r fairground_cache.zip fairground_cache
```
