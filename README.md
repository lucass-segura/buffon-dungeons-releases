# Buffon Dungeons - downloads

Buffon Dungeons is a dungeon poker roguelike for the desktop: play poker hands to deal damage, beat a monster on
every floor, and build a deck of jesters and sigils. Solo, or online with up to three friends.

This repository only holds the installers (see **Releases**). The game is not open source and no source code is
published here.

## Install

Download the file for your system from the [latest release](../../releases/latest).

**Windows**
- `Buffon-Dungeons-<version>-windows-setup.exe`: run it and follow the pages (no administrator rights needed).
- Or `Buffon-Dungeons-<version>-windows.zip`: unzip anywhere and run `Buffon Dungeons.exe`.
- The build is not code-signed, so SmartScreen may say "Windows protected your PC". Choose **More info**, then
  **Run anyway**.

**macOS** (recommended: one line in Terminal)
```
curl -fsSL https://github.com/lucass-segura/buffon-dungeons-releases/releases/latest/download/install-macos.sh | bash
```
- It downloads the latest `.dmg`, verifies its SHA-256, copies the game to Applications and opens it. No warning from
  macOS, no administrator password.
- Or open `Buffon-Dungeons-<version>-macos.dmg` and drag **Buffon Dungeons** to Applications. The build is not notarized
  by Apple, so the first launch shows "Apple could not verify…": click **Done** (not Move to Trash), open
  **System Settings > Privacy & Security**, scroll to the bottom and choose **Open Anyway**, then confirm. Only once.

**Linux (x86_64)**
- `tar xzf Buffon-Dungeons-<version>-linux-x86_64.tar.gz`, then run `./install.sh` inside the folder (installs for
  your user and adds a menu entry; `./uninstall.sh` removes it). Or run `./buffon-dungeons` without installing.
- The AppImage needs FUSE; without it the launcher extracts and runs.

## Updates

The game checks this repository for a newer version when you open the menu and offers to update itself ("Download
now"). The download is verified with a SHA-256 checksum before it is used. `SHA256SUMS` in every release lets you
check the installers yourself: `shasum -a 256 -c SHA256SUMS` (macOS, Linux) or `Get-FileHash` (Windows).

## Rights

Copyright (c) Buffon Dungeons. All rights reserved. The installers are provided to play the game; no licence is
granted to copy, modify, decompile or redistribute the game. The game runs on [LOVE](https://love2d.org), which is
distributed under the zlib licence (included in the installers).

## En español

Buffon Dungeons es un roguelike de póker en mazmorras para escritorio. Descarga el archivo de tu sistema desde la
[última versión](../../releases/latest).

- **Windows:** ejecuta el `-setup.exe` (o descomprime el `.zip` y abre `Buffon Dungeons.exe`). Como la compilación no
  está firmada, SmartScreen puede mostrar un aviso: elige **Más información** y luego **Ejecutar de todas formas**.
- **macOS (recomendado):** pega esto en Terminal:
  `curl -fsSL https://github.com/lucass-segura/buffon-dungeons-releases/releases/latest/download/install-macos.sh | bash`
  (descarga, verifica e instala el juego sin avisos). O abre el `.dmg` y arrastra el juego a Aplicaciones; como no está
  notarizado por Apple, la primera vez aparece "Apple no pudo verificar…": pulsa **Listo** (no "Mover al basurero"), ve a
  **Ajustes del Sistema > Privacidad y seguridad**, baja hasta el final, pulsa **Abrir igualmente** y confirma. Solo la primera vez.
- **Linux (x86_64):** descomprime el `.tar.gz` y ejecuta `./install.sh`.

El juego busca versiones nuevas al abrir el menú y se actualiza solo (la descarga se verifica con SHA-256). Todos los
derechos reservados: el juego no es de código abierto y no se publica su código fuente.
