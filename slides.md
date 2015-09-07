# Team Hopper
### Cranny, Fraser, Shen, Spearritt

---


## Tile Engine

- Core Engine
- Generation & Rendering
- Storage & Persistence
- Collision & Interaction


---

## Core Engine

- `Tile` | `TileChunk` | `TileGridManager`
-  Each tile uses one byte of storage space

---

## Generation & Rendering

- Fixed-size world generated on first launch
- Generation techniques interchangeable through `TileGenerator` interface
- Rendered (with texture assets!) selectively based on 'world offset' position

---

## Storage & Persistence

- Persisted in the database
- BLOB!
- ???

---

## Collision & Interaction

- Entities collide with solid tiles much as with other entities
- Tile collision more efficient, as checking is restricted to area surrounding an entity
- Other interactions (mining etc.): Tile are stateless

---

## New Slide
- Dot
- Points
- Here

--

## Sub-Slide
![asd](media/joe.jpg)

Note: This shows up in the speaker notes.

