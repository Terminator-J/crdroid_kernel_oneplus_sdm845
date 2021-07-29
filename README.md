## Hola amiguitos

This is my attempt to fix up and add a little crDroid customization flavor back into the sdm845 kernel tree for OnePlus 6 & 6T (enchilada & fajita).

Rebased on the official lineage-18.1 branch from LineageOS as of July 2021, with some extra goodies added in like clang-12 support, multiple vibration type support, wireguard support, and battery-idle-mode-enabled charging switches.

Dropping my DC dimming (LOS Anti Flicker) commit for now because until they decide to rebase the display/panel handling on OOS Q or later, it will never be compatible with updated FOD handling as currently exists.
