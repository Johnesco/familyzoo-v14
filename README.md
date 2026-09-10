# Family Zoo — v14 — Capability Dispatch

Petting the goats feels different from petting the parrot (which bites). Introduces capability dispatch — one verb whose behavior is delegated to whichever trait the target entity carries.

Step 14 of the [Family Zoo](https://github.com/Johnesco/familyzoo) tutorial — a progressive walkthrough of the [Sharpee](https://sharpee.net) TypeScript interactive fiction engine, from a single room to a full multi-file story.

## What this step teaches

- Custom traits declaring a static capabilities[] list
- registerCapabilityBehavior with optional condition predicates
- createCapabilityDispatchAction factory for auto-built dispatch actions
- Per-entity behavior selection via trait data like animalKind
- The verb vs entity responsibility split vs. plain custom actions

## Playing

Open `play.html`, or preview the folder:

```bash
python -m http.server 8000 --directory familyzoo-v14
```

## Building

This is a **frozen 0.9.x TypeScript version**. The built player in this folder is the published artifact; it is re-laid from `browser/` by the workspace build:

```bash
python ../tools/build.py familyzoo-v14
python C:/code/ifhub/tools/ship.py familyzoo-v14
```

The authoring tree for every version lives in the [familyzoo](https://github.com/Johnesco/familyzoo) repo.
