# NZP PS3 community map catalog

Replacement catalog for Nazi Zombies: Portable PS3, tested against the catalog parser in build `2.0.2-preview+ps3-1f0ac20`. The original developer repository is unavailable.

## Use it

Add this line to `/dev_hdd0/game/NZPP00001/USRDIR/nzp/autoexec.cfg`, then restart NZP:

```cfg
ps3_maps_url "https://raw.githubusercontent.com/richard1222/nzp-maps/refs/heads/main/maps.json"
```

Open **Download Maps** in the main menu.

## Available entries

- Nacht der Untoten — existing initial test entry, NZ:P Team.
- [Kino der Toten](https://github.com/nzp-team/nzportable/discussions/708) — MotoLegacy, LexiAshe and DerpedCrusader.
- [Andes](https://github.com/nzp-team/nzportable/discussions/772) — vichoca9 (map metadata credits Striga).
- [Shipment Survival](https://github.com/nzp-team/nzportable/discussions/1513) — Blake-Izayoi.

The three new entries point directly to downloads published by their authors. Their ZIP integrity, expected BSP files, archive paths, byte sizes and SHA-256 hashes were checked before listing. The catalog schema and absolute-URL support were verified against the installed PS3 executable. This does **not** establish PS3 download or gameplay compatibility; console testing is pending.

Map content belongs to its authors. This catalog is not affiliated with or endorsed by the NZ:P Team. Existing `ndu.zip` remains from the initial test; no additional map archives are mirrored here.

## Maintenance

Keep `file` as the author-published ZIP URL and verify `size`, `sha256` and `bsp` after any upstream archive change. The PS3 parser accepts a `maps` array and optional name, author, version, size, description, date and thumbnail fields; descriptions may contain up to six lines. Catalog validation does not guarantee a custom map will run correctly.
