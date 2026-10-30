# 3d-inventory-schema

The engine-independent form of an item container, as JSON Schema 2020-12 (`inventory.schema.json`).

A container has a slot count, a stack limit and a list of items by id and total quantity. The schema does not say what an item is: ids belong to the game. Any runtime can read and write it; the Unity adapter is [`3d-unity-inventory`](../3d-unity-inventory).

`examples/backpack.json` is a valid container.

### Status

v1 draft: one container shape, one example.

### Roadmap

- Invalid fixtures and a validation script.
- Per-item stack limits and item metadata, if a second runtime needs them.
