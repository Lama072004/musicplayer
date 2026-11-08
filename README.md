# Musicplayer

Deutsch | [English](#english)

> **Status: in Planung.** Das Projekt ist aktuell nur das Flutter-Grundgerüst. Dieses Dokument beschreibt das Ziel, nicht den heutigen Stand.

Ein Streaming-Client für den eigenen **[Navidrome](https://www.navidrome.org/)**-Server, der aussieht und sich bedient wie Spotify. Die Musik bleibt auf dem eigenen Server, die App ist nur die Oberfläche dafür.

## Idee

Bestehende Subsonic-/Navidrome-Apps (z. B. Substreamer) funktionieren gut, wirken aber oft nüchtern. Dieses Projekt soll entweder

- eine bestehende Open-Source-App wie Substreamer als Ausgangspunkt umbauen **oder**
- einen eigenen Client in Flutter von Grund auf bauen,

jeweils mit einer Bedienung, die man von Spotify kennt. Welcher der beiden Wege es wird, ist noch offen.

## Geplante Funktionen

- Anmeldung am eigenen Navidrome-Server (Subsonic-API)
- Startseite mit Zuletzt gehört, Neu hinzugefügt und Empfehlungen
- Bibliothek: Künstler, Alben, Titel, Playlists, Favoriten
- Suche über die gesamte Bibliothek
- Player mit Mini-Player, Vollbild-Ansicht, Warteschlange, Shuffle und Wiederholen
- Wiedergabe im Hintergrund mit Steuerung über Sperrbildschirm und Benachrichtigung
- Cover-Darstellung und dynamische Farben passend zum Album
- Offline-Modus mit heruntergeladenen Titeln
- Scrobbling zum Server
- Hell/Dunkel

Die Liste ist ein Entwurf und wird angepasst, sobald der Weg (Umbau oder Neubau) feststeht.

## Technik

- Flutter (Dart SDK `^3.9.2`)
- Server: Navidrome über die Subsonic-kompatible API
- Plattformen: zuerst Android, das Projekt ist als Flutter-Projekt auch für iOS, Web, Windows, Linux und macOS angelegt

## Entwickeln

```bash
flutter pub get
flutter run
```

## Lizenz

Noch nicht festgelegt. Falls eine bestehende App als Grundlage dient, gilt deren Lizenz.

---

## English

# Musicplayer

> **Status: planned.** The project is currently just the Flutter scaffold. This document describes the goal, not the current state.

A streaming client for your own **[Navidrome](https://www.navidrome.org/)** server that looks and feels like Spotify. The music stays on your own server; the app is just the interface.

### Idea

Existing Subsonic/Navidrome apps (e.g. Substreamer) work well but often feel plain. This project will either

- take an existing open-source app such as Substreamer as a starting point and rework it, **or**
- build an own client in Flutter from scratch,

in both cases with an interface familiar from Spotify. Which of the two it will be is still open.

### Planned features

- Sign-in to your own Navidrome server (Subsonic API)
- Home screen with recently played, recently added and recommendations
- Library: artists, albums, tracks, playlists, favorites
- Search across the whole library
- Player with mini player, full-screen view, queue, shuffle and repeat
- Background playback with lock-screen and notification controls
- Cover art display and dynamic colors matching the album
- Offline mode with downloaded tracks
- Scrobbling to the server
- Light/dark

This list is a draft and will be adjusted once the path (rework or rebuild) is decided.

### Tech

- Flutter (Dart SDK `^3.9.2`)
- Server: Navidrome via the Subsonic-compatible API
- Platforms: Android first; the Flutter project is also set up for iOS, web, Windows, Linux and macOS

### Development

```bash
flutter pub get
flutter run
```

### License

Not decided yet. If an existing app is used as a base, its license applies.
