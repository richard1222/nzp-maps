# nzp-maps

Community mirror for the map list of the Nazi Zombies Portable PS3 port
("Vril Engine PS3", build 2.0.2-preview+ps3-1f0ac20 by daedra000).

The port's downloader fetches its map list from a GitHub repository that no
longer exists, so Download Maps fails with a 404. This repo hosts a
replacement `maps.json` plus repacked map zips. The game can be pointed at
it without any binary patch via the `ps3_maps_url` console variable in
`nzp/autoexec.cfg`.

EXPERIMENTAL: the maps.json schema is being reverse-engineered from the
game binary and runtime log feedback. The current file is a best-guess
first candidate and may change.

Maps are repacked from files already installed on the console by the
community; no original game assets are redistributed here beyond what the
port itself installed. Map content belongs to its original authors
(Nacht der Untoten: NZ:P Team).
