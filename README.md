# interactor-multiplayer-fabric-elf-programs

Sandboxed RISC-V guest programs for the multiplayer fabric: grid simulation kernels and an HTN planner with holographic memory.

## What it is for

Each program is a thin wrapper that exposes simulation or planning functions to the engine's sandbox host. The logic lives in header-only code in sibling repositories, which the build expects beside this checkout. Changing a public kernel symbol means changing the host's binding table at the same time. `AGENTS.md` and `CONTRIBUTING.md` carry the working notes.

## Build and run

```sh
scons
```

The build finds a RISC-V cross compiler on its own.

## Licence

The licence is not stated.
