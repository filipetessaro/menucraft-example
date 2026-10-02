# Menucraft Example

Example project for **Menucraft**, the gamepad-first CommonUI menus, settings and loading screen plugin for Unreal
Engine. It is Epic's Third Person template set up exactly as Menucraft's Quick start describes. Blueprint only, no
C++ and no Visual Studio needed.

**Download:** [MenucraftExample_UE5.6.zip](https://github.com/filipetessaro/menucraft-example/releases/latest)
(Releases, on the right). Made in UE 5.6; opens in 5.6, 5.7 and 5.8.

## Use it

1. Install Menucraft from Fab into your engine (5.6, 5.7 or 5.8). The plugin is not included here.
2. Unzip and open `MenucraftExample.uproject`.
3. Press Play. The main menu opens over the level; Play loads the level (the loading screen shows in Standalone Game
   and packaged builds); Escape or the controller's Start opens the pause menu.

## What's in it

- `Content/MenucraftExample/BP_MenucraftPlayerController`, which the template's game mode spawns:
  - **Event Graph:** Play opens the level; the Field of View setting is applied now and whenever settings change;
    on the menu it shows the main menu, and in the game it holds the loading screen until it's set up.
  - **Pause:** Escape or Start calls Show Pause (with Execute when Paused).
  - **Settings:** applies the Field of View custom setting to the character's camera.
- `Config/`: the Quick start lines (DefaultEngine, DefaultGame, DefaultInput) and Menucraft's settings (also in
  Project Settings > Plugins > Menucraft): the template's input contexts as Remappable Contexts, a Field of View
  custom setting, credits, loading tips, every preset theme for the player to choose, and the ten translations staged
  for packaging.

## Links

- Documentation: https://apps.tessaroapps.com/menucraft/docs/
- Support: contato@tessaroapps.com

The Third Person template content is Epic Games' and is used under the Unreal Engine EULA. Menucraft is sold on Fab and
is not part of this download.
