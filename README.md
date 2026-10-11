# 🚬 Cigar Mod for Minecraft Java (26.x)

A Fabric mod for Minecraft Java Edition that adds a complete tobacco economy to the game: grow
it, harvest it, dry it, and finally roll it into cigarettes or cigars — including a whole range
of decorative building blocks.

> ⚠️ **Disclaimer:** This mod portrays tobacco use in an exaggerated, satirical way and is not
> meant to encourage smoking. Smoking is unhealthy — in Minecraft and in real life.

## 📦 Project structure

- [`Cigar-Mod/`](Cigar-Mod) – the current, actively developed mod project (target: Minecraft Java
  **26.x**, Fabric).
- [`Cigar-Mod-1.21/`](Cigar-Mod-1.21) – the old 1.21 version of the mod. Kept only as a
  **reference** for features from an earlier project phase and no longer actively developed.

## ✨ Features

### 🌱 Growing tobacco
- A new crop, **tobacco** (`tobacco_crop`), planted with tobacco seeds (`tobacco_seeds`) on
  farmland. It grows through several stages and, once fully grown, is harvested into
  **tobacco leaves** (`tobacco_leaf`).

### 🧵 Drying rack
- Build your own drying rack out of **fences** (vanilla or modded) and the new **tobacco
  string** block (`tobacco_string`), crafted from regular string.
- The tobacco string can:
  - be placed directly next to a fence, **or**
  - hang from another tobacco string that is (directly, or through an arbitrarily long chain of
    further strings) eventually connected to a fence.
  - In either case, the string must have **at least 1 block of clearance above the ground**
    (ground → air → string, or even more air) — it can't simply be placed flat on the ground like
    a carpet.
- Right-click with a tobacco leaf in hand to hang the leaf on the string.
- The leaf dries over time (random-tick based, similar to crops) through several stages.
- Once fully dried, right-click to harvest it as a **dried tobacco leaf** (`dried_tobacco_leaf`).
- Alternatively, a tobacco leaf can also be "dried" the classic way by smelting it in a furnace.

### 🚬 Cigarettes
- Crafted from paper + a dried tobacco leaf.
- Short smoking duration, grants a brief burst of speed (and has a small chance of causing
  nausea).

### 📦 Cigarette box
- Crafted from **9 cigarettes**.
- **Right-clicking the box splits it back into 9 individual cigarettes** — handy for storage and
  stacking.
- 9 cigarette boxes can be crafted into a **cigarette box block**, which in turn unlocks a full
  building set: stairs, slabs, a door, a trapdoor, a fence, a fence gate, a wall, a button and a
  pressure plate.

### 🚬 Cigars
- Crafted from paper + a dried tobacco leaf + a sponge.
- Long smoking duration, grants speed, but also has a chance of causing nausea or wither.
- Leaves behind a **cigar stub** (`cigar_stub`) after smoking, which can be used as furnace fuel
  (just like a stick).
- 9 cigars can be crafted into a **block of cigars**, which also unlocks a full building set:
  stairs, slabs, a door, a trapdoor, a fence, a fence gate, a wall, a button and a pressure plate.

## 🎯 Target version

The mod targets the entire **Minecraft Java 26.x** release line (currently tested against 26.3)
and uses [Fabric Loader](https://fabricmc.net/) + [Fabric API](https://github.com/FabricMC/fabric).

> Note: The exact Yarn mapping / Fabric API build numbers in
> [`Cigar-Mod/gradle.properties`](Cigar-Mod/gradle.properties) should be checked/updated against
> [fabricmc.net/develop](https://fabricmc.net/develop) once official builds for 26.x are released.

## 🛠️ Build

```powershell
cd Cigar-Mod
./gradlew build
```

The finished mod jar will be located at `Cigar-Mod/build/libs/`.

## 📜 License

See [`LICENSE`](LICENSE).

