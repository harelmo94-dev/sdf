# Krypton Client

Fabric · Minecraft **1.21.11** · Java 21 (runtime) · Yarn mappings 1.21.11+build.4

## Build
- GitHub: push the repo, open Actions -> latest run -> Artifacts -> `krypton-client-1.21.11` (jar inside).
- Local: JDK 25 (what the Fabric example mod uses for building) then `./gradlew build`; jar in `build/libs/`
  (use `krypton-client-0.2.0.jar`, not `-sources`).

## Install
Minecraft 1.21.11 + Fabric Loader + Fabric API (0.141.x for 1.21.11) + this jar in `.minecraft/mods`.

## Controls
- Right Shift: open/close ClickGUI (rebindable)
- Module: left-click toggle · right-click expand settings · middle-click bind key (Backspace clears)
- Window header: drag to move · right-click to collapse
- Type while the GUI is open to filter modules
- Config: .minecraft/krypton/config.json

## Contents
- Core: EventBus, ModuleManager (keybinds, Panic kill-switch), Setting system, JSON config
- ClickGUI: draggable animated windows, search, tooltips, key binding, sliders/toggles
- HUD: watermark, FPS, ping, speed, coords, animated ArrayList, toggle notifications
- Modules: ClickGUI, HUD, Panic, Sprint, AutoWalk, Fullbright
