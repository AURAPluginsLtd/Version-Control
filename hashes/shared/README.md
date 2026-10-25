# Shared hash manifests

`shared` is the Download Manager's own binary and the data files every product uses. Editor standalone apps stay in `demo/` and `full/` with their plugins.

No Download Manager hashes are published here yet. When they are, the file name matches the other tiers: `<product>-<mac|pc>-hashes.json`. The document is schema 2, the same shape as `full/` and `demo/`: a `builds` array, one object per version. A new build is appended. The same version replaces that one object, and older builds stay. The app treats a missing file as an empty list.
