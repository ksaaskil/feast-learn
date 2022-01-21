# Feast Feature Store

```bash
$ pip install -e .
```

Created the feature store repository with:

```bash
$ feast init feature_repo
```

Applied `example.py` with:

```bash
$ cd feature_repo
$ feast apply
```

Materialized to online store with:

```bash
$ CURRENT_TIME=$(date -u +"%Y-%m-%dT%H:%M:%S")
$ feast materialize-incremental $CURRENT_TIME
```
