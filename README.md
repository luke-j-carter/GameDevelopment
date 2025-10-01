# Unreal Gameplay Engineer — Labs & Capstone

Hands-on Unreal Engine 5 C++ course repo focused on **GAS**, **networking/replication**, **AI (BT/EQS/StateTree)**, **UI/Save**, and **performance**. Built as a portfolio-ready project with weekly labs, tests, and profiling.

## What’s inside
- **/Source** – C++ gameplay code (abilities, components, replication)
- **/Content** – assets (organized by feature folders)
- **/Plugins** – tools/plugins (e.g., RogueGAS Utils, Pipeline Tools)
- **/Tests** – AutomationSpec & Functional test maps
- **/Docs** – short technical notes (Perf.md, Net.md, AI.md) + GIFs
- **/Scripts** – build/cook helpers (UAT), pre-commit, formatting

## Getting started
1. UE 5.5, Visual Studio/CLion/Xcode set up  
2. Clone → open `*.uproject` → enable: **GameplayAbilities**, **GameplayTags**, **GameplayTasks**
3. Optional: install Git LFS (`*.uasset`, `*.umap`)

```bash
# Format (optional)
clang-format -i Source/**/*.h Source/**/*.cpp

# Run tests (headless)
UE5Editor-Cmd.exe Project.uproject -ExecCmds="Automation RunTests Project.*; Quit"
