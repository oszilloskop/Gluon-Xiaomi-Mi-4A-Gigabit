# Gluon v2021.1.x Patches für "Xiaomi Mi Router 4A Gigabit Edition"
In dem Thread: [https://forum.freifunk.net/t/xiaomi-4a-gigabit-mt7621-mit-ac-fuer-20-backport-auf-gluon2021-1-x-verfuegbar/23014](https://forum.freifunk.net/t/xiaomi-4a-gigabit-mt7621-mit-ac-fuer-20-backport-auf-gluon2021-1-x-verfuegbar/23014) werden Patches und Skripte für den Bau eines Gluon-Images für den Router "Xiaomi Mi Router 4A Gigabit Edition" aufgeführt. Danke an @Adorfer.


Da ich eine eigene Build-Umgebung pflege, welche nicht wirklich auf Fremd-Skripte vorbereitet ist, habe ich mal alles mit Patches gelöst. Die Patches basieren komplett auf den oben erwähnten Thread.

---
### Die Patches habe ich erfolgreich unter Gluon v2021.1.2 angewendet
---

Die hier enthaltenen Patches können händisch oder automatisiert eingespielt werden.


Für das Anwenden der einzelnen Patches verwende ich jeweils folgenden Befehl:

`patch -N -p1 -r - -s -i ./VerzeichnisPfad/PatchNameXY`

Die Patches müssen mind. einmal nach dem Aufruf von `make update` angewendet werden. Ein wiederholtes Patchen ist unkritisch.

Die Patches sind so aufgebaut, dass das Patchen im Grundverzeichnis der Gluon-Buildumgebung durchgeführt werden muß.
