# Ghost Exile Russian Language Fix for CrossOver

This repository contains a shell script for fixing the Russian language setup for `Ghost Exile` when the game is installed through Steam inside CrossOver on macOS.

## What the script does

- switches the Steam app language metadata for `Ghost Exile` to Russian
- updates the per-user Steam config for the game
- fixes the internal game language value in the CrossOver bottle registry
- creates fallback localization folders for broken in-game language mappings

## Usage

```bash
chmod +x ghost_exile_ru_crossover.sh
./ghost_exile_ru_crossover.sh --kill-steam --start-steam
```

## Notes

- the script is intended for one-time repair, not for permanent background use
- it creates backup copies before changing Steam or bottle files
