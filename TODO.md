# TODO

## Pass 1 — Infrastructure

- [x] Add KiBot/docs pipeline
- [x] Confirm DRC passes in CI
- [ ] Confirm ERC passes in CI — **92 warnings (see below)**
- [ ] Verify board renders generate correctly (blocked by ERC/Fab failure)

### ERC Issues (from CI run 26140176787)
- Missing library: `SparkFun-LED` (footprint + symbol)
- Missing library: `SparkFun-DiscreteSemi` (symbol)
- Missing library: `kml-custom` (footprint + symbol, multiple refs)
- Symbol mismatch: `+12V`, `GND` don't match `power` library
- Symbol not found: `Conn_01x10_Female` in `Connector` library
- Pin type warnings: Unspecified-to-Unspecified in ADM3260 sub-sheet
- Missing footprint component: `SparkFun-LED:WS2812B_5050`

## Pass 2 — Pre-Fab Review

- [ ] Full ERC/DRC clear
- [ ] BOM review and sourcing check
- [ ] Footprint verification against datasheets
- [ ] Design review sign-off
