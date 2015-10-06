# Team Hopper
### Cranny, Fraser, Shen, Spearritt
## Critique 2
---

## Last time, on *Team Hopper*...

- Tile Engine
-- Tile Generation
-- Tile Persistence
-- Tile Rendering
-- Tile Interaction

---

## Since then...

- Tile Engine improvements
- Modifiers / World Gen Pipeline
- Test improvements
- Misc. additions

--

### Tile Engine

- More database stuff?

--

### World Generation Pipeline (#88)

- `TileModifier` interface, and `TileGridManager` infrastructure
- Modifiers created so far - `SquareVeinTileModifier` and `PerlinVeinTileModifier`
- Associated `NoiseCreator` class for creating Perlin noise / fractal noise (with Fractal Brownian Motion)

--

```
double pX, pY;
pX = (((double)globalX / 2000.0) * noiseGridSize) - noiseGridSize/2;
pY = (((double)globalY / 2000.0) * noiseGridSize) - noiseGridSize/2;
double perlin = noiseCreator.getPerlin(pX, pY);
if (perlin >= RUBY_THRESHOLD) {
	chunk.setTileType(x, y, Tile.RUBY);
} else if (perlin <= DIAMOND_THRESHOLD) {
	chunk.setTileType(x, y, Tile.GOLD);
}
```

--

### Testing improvements

- Assorted tile testing improvements
- Tile rendering now tested thanks to PowerMock

--

### Other Additions / Involvement

- Made vertical mouse panning work
- Added parallax effect to the sun
- Work towards making the game resizeable

---

## Challenges

- WorldGen: noise generation
-- Noise that 'looks right'
-- Testing fundementally random processes
- Mouse panning: World had no concept of 'y offset', and rendering was written assuming the y position was fixed
- ???

---

## What's Next?

???

---

## Call for Feedback

- ???
	
---

## Questions?