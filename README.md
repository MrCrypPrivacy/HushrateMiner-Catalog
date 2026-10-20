# Hushrate Miner package catalog

Package catalog for [Hushrate Miner](https://github.com/MrCrypPrivacy/HushrateMiner-x-Logos-Basecamp),
solo Monero mining for [Logos Basecamp](https://logos.co).

## Add the catalog to Basecamp

1. Open Basecamp and go to Package Manager, then Add repository
2. Paste this URL:

```
https://raw.githubusercontent.com/MrCrypPrivacy/HushrateMiner-Catalog/refs/heads/main/logos-repo.json
```

3. Install `hushrate_miner`. The core module `hushrate_core` is installed automatically as a
   dependency

## Packages

| Package | Type | Purpose |
| --- | --- | --- |
| `hushrate_core` | core | Downloads and verifies XMRig and P2Pool, runs and controls them |
| `hushrate_miner` | ui_qml | User interface |

New versions are added to the index as they are released, and older versions stay listed.

## Files

| File | Purpose |
| --- | --- |
| `logos-repo.json` | Catalog description. This is the file Basecamp reads first |
| `index.json` | Package listing with versions, download URLs and hashes. Generated, do not edit by hand |
| `icons/` | Package icons referenced by `index.json` |

The packages themselves are not stored here. Each entry in `index.json` points to the
`.lgx` file attached to the matching release of the project repository, and Basecamp checks
the download against the hashes in the index before installing it.
