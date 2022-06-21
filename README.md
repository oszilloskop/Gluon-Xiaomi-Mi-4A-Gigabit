# Gluon v2021.1.x Patches für "Xiaomi Mi Router 4A Gigabit Edition"
In dem Thread: [https://forum.freifunk.net/t/xiaomi-4a-gigabit-mt7621-mit-ac-fuer-20-backport-auf-gluon2021-1-x-verfuegbar/23014](https://forum.freifunk.net/t/xiaomi-4a-gigabit-mt7621-mit-ac-fuer-20-backport-auf-gluon2021-1-x-verfuegbar/23014) werden Patches und Skripte für den Bau eines Gluon-Images für den Router "Xiaomi Mi Router 4A Gigabit Edition" aufgeführt. Danke dafür an @Adorfer.


Da ich eine eigene Build-Umgebung pflege, welche nicht wirklich auf Fremd-Skripte vorbereitet ist, habe ich mal alles mit Patches gelöst. Die Patches basieren komplett auf dem oben erwähnten Thread.

---
### Die Patches habe ich erfolgreich unter Gluon v2021.1.2 angewendet
---

Die hier enthaltenen Patches können händisch oder automatisiert eingespielt werden.


Für das Anwenden der einzelnen Patches verwende ich jeweils folgenden Befehl:

`patch -N -p1 -r - -s -i ./VerzeichnisPfad/PatchNameXY`

Die Patches müssen mind. einmal nach dem Aufruf von `make update` angewendet werden. Ein wiederholtes Patchen ist unkritisch.

Die Patches sind so aufgebaut, dass das Patchen im Grundverzeichnis der Gluon-Buildumgebung durchgeführt werden muß.

---

Beim Bau des `ramips-mt7621` Targets wird dann ein Sysupgrade-Image für den Xiaomi Mi Router 4A Gigabit Edition erzeugt. 

---

### Patchfiles im Raw-Format
[001-add-mi-router-4a-gigabit-gluon.patch](/001-add-mi-router-4a-gigabit-gluon.patch?raw=true)  
[002-add-mi-router-4a-gigabit-openwrt.patch](002-add-mi-router-4a-gigabit-openwrt.patch?raw=true)  
[003-XIAOMI-MIR4A-GIGABIT.dts.patch](003-XIAOMI-MIR4A-GIGABIT.dts.patch?raw=true)  
[004-u-boot-upgrade.patch](004-u-boot-upgrade.patch?raw=true)  
[005-690-net-add-support-for-threaded-NAPI-polling.patch.patch](005-690-net-add-support-for-threaded-NAPI-polling.patch.patch?raw=true)  
