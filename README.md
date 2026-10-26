# Miro Tools

Internal Miro Web SDK tools.

## Structure

```text
miro-tools/
├─ README.md
└─ ssot-sync/
   └─ index.html
```

## Tools

### SSOT Sync

Manual canonical → reference linking for Miro objects.

- Canonical sources live inside the `Ontology` frame.
- Select 2 shapes to create or repair a link.
- Deselect everything and run Sync to update all registered references.
- Links are stored in board-level AppData.
- No text matching, board scanning, aliases, or frame-based search.

Miro SDK path after repository migration:

```text
https://alexandrsemenuk.github.io/miro-tools/ssot-sync/?build=v7
```

## Deployment

GitHub Pages:
- Branch: `main`
- Folder: `/ (root)`

Each tool lives in its own folder and is connected to its own Miro App through `sdkUri`.

Use a new cache-busting query parameter after meaningful releases:

```text
?build=v7
?build=v8
?build=v9
```
