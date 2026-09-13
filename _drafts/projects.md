---
layout: post
title: "What I Build: A Tour of My Projects"
description: "Nine things I built, from desktop apps for my Linux setup to civic dashboards and a research tool, each with a schematic card that shows what it does at a glance."
categories:
- Projects
tags:
- portfolio
- linux
- gtk4
- nextjs
- open-data
- design
media_subpath: /assets/img/projects/
author: felix
pin: true
---

Most of what I build starts as something I wanted for myself: a screenshot
tool that behaves the way I remember from Windows, a dictionary for the
Japanese I am learning, a mail client that opens instantly. Some of it grew
into things other people can use, some of it stays a tool for one person.
This is the overview: the gallery for a glance, the sections below for a paragraph each. Every project has, or will get, a post of its own.

Every project carries the same two marks: a small icon, and a schematic
"card" that shows the shape of the app rather than a screenshot. The cards
are deliberately abstract, one dark frame, a muted outline of the interface,
and one lit detail that says what the project is about. Together they are
the visual thread through everything below.

<div style="display:grid;grid-template-columns:repeat(auto-fill,minmax(230px,1fr));gap:14px;margin:1.5rem 0 2.5rem">
  <a href="#snip-pin" style="display:block;text-decoration:none;color:inherit;border:1px solid var(--card-border-color, #ddd);border-radius:12px;overflow:hidden;background:var(--card-bg, transparent)">
    <img src="/assets/img/projects/snip-pin/card.png" alt="" style="display:block;width:100%;aspect-ratio:16/9;object-fit:cover;margin:0">
    <span style="display:flex;align-items:center;gap:10px;padding:10px 12px">
      <img src="/assets/img/projects/snip-pin/icon.svg" alt="" style="width:36px;height:36px;flex:none;margin:0">
      <span style="display:flex;flex-direction:column;line-height:1.25"><strong>snip-pin</strong><small style="opacity:.75">Snip and pin for Hyprland</small></span>
    </span>
  </a>
  <a href="#tango" style="display:block;text-decoration:none;color:inherit;border:1px solid var(--card-border-color, #ddd);border-radius:12px;overflow:hidden;background:var(--card-bg, transparent)">
    <img src="/assets/img/projects/tango/card.png" alt="" style="display:block;width:100%;aspect-ratio:16/9;object-fit:cover;margin:0">
    <span style="display:flex;align-items:center;gap:10px;padding:10px 12px">
      <img src="/assets/img/projects/tango/icon.svg" alt="" style="width:36px;height:36px;flex:none;margin:0">
      <span style="display:flex;flex-direction:column;line-height:1.25"><strong>Tango 単語</strong><small style="opacity:.75">Japanese dictionary for GNOME</small></span>
    </span>
  </a>
  <a href="#den-mail" style="display:block;text-decoration:none;color:inherit;border:1px solid var(--card-border-color, #ddd);border-radius:12px;overflow:hidden;background:var(--card-bg, transparent)">
    <img src="/assets/img/projects/den-mail/card.png" alt="" style="display:block;width:100%;aspect-ratio:16/9;object-fit:cover;margin:0">
    <span style="display:flex;align-items:center;gap:10px;padding:10px 12px">
      <img src="/assets/img/projects/den-mail/icon.svg" alt="" style="width:36px;height:36px;flex:none;margin:0">
      <span style="display:flex;flex-direction:column;line-height:1.25"><strong>Den Mail</strong><small style="opacity:.75">Fastmail client for GNOME</small></span>
    </span>
  </a>
  <a href="#yubioath-gtk" style="display:block;text-decoration:none;color:inherit;border:1px solid var(--card-border-color, #ddd);border-radius:12px;overflow:hidden;background:var(--card-bg, transparent)">
    <img src="/assets/img/projects/yubioath-gtk/card.png" alt="" style="display:block;width:100%;aspect-ratio:16/9;object-fit:cover;margin:0">
    <span style="display:flex;align-items:center;gap:10px;padding:10px 12px">
      <img src="/assets/img/projects/yubioath-gtk/icon.svg" alt="" style="width:36px;height:36px;flex:none;margin:0">
      <span style="display:flex;flex-direction:column;line-height:1.25"><strong>YubiOath</strong><small style="opacity:.75">YubiKey codes for GNOME</small></span>
    </span>
  </a>
  <a href="#knx-panel" style="display:block;text-decoration:none;color:inherit;border:1px solid var(--card-border-color, #ddd);border-radius:12px;overflow:hidden;background:var(--card-bg, transparent)">
    <img src="/assets/img/projects/knx-panel/card.png" alt="" style="display:block;width:100%;aspect-ratio:16/9;object-fit:cover;margin:0">
    <span style="display:flex;align-items:center;gap:10px;padding:10px 12px">
      <img src="/assets/img/projects/knx-panel/icon.svg" alt="" style="width:36px;height:36px;flex:none;margin:0">
      <span style="display:flex;flex-direction:column;line-height:1.25"><strong>Control-9 Wandpanel</strong><small style="opacity:.75">Home Assistant on a 2008 wall panel</small></span>
    </span>
  </a>
  <a href="#color-combinator" style="display:block;text-decoration:none;color:inherit;border:1px solid var(--card-border-color, #ddd);border-radius:12px;overflow:hidden;background:var(--card-bg, transparent)">
    <img src="/assets/img/projects/color-combinator/card.png" alt="" style="display:block;width:100%;aspect-ratio:16/9;object-fit:cover;margin:0">
    <span style="display:flex;align-items:center;gap:10px;padding:10px 12px">
      <img src="/assets/img/projects/color-combinator/icon.svg" alt="" style="width:36px;height:36px;flex:none;margin:0">
      <span style="display:flex;flex-direction:column;line-height:1.25"><strong>Color Combinator</strong><small style="opacity:.75">Sanzo Wada's colour dictionary</small></span>
    </span>
  </a>
  <a href="#civic-digital" style="display:block;text-decoration:none;color:inherit;border:1px solid var(--card-border-color, #ddd);border-radius:12px;overflow:hidden;background:var(--card-bg, transparent)">
    <img src="/assets/img/projects/civic-digital/card.png" alt="" style="display:block;width:100%;aspect-ratio:16/9;object-fit:cover;margin:0">
    <span style="display:flex;align-items:center;gap:10px;padding:10px 12px">
      <img src="/assets/img/projects/civic-digital/icon.svg" alt="" style="width:36px;height:36px;flex:none;margin:0">
      <span style="display:flex;flex-direction:column;line-height:1.25"><strong>Civic Digital</strong><small style="opacity:.75">One place, one page of open data</small></span>
    </span>
  </a>
  <a href="#cultural-distances" style="display:block;text-decoration:none;color:inherit;border:1px solid var(--card-border-color, #ddd);border-radius:12px;overflow:hidden;background:var(--card-bg, transparent)">
    <img src="/assets/img/projects/cultural-distances/card.png" alt="" style="display:block;width:100%;aspect-ratio:16/9;object-fit:cover;margin:0">
    <span style="display:flex;align-items:center;gap:10px;padding:10px 12px">
      <img src="/assets/img/projects/cultural-distances/icon.svg" alt="" style="width:36px;height:36px;flex:none;margin:0">
      <span style="display:flex;flex-direction:column;line-height:1.25"><strong>Cultural Distances</strong><small style="opacity:.75">Hofstede and the Culture Map, measured</small></span>
    </span>
  </a>
  <a href="#bottleneck-sim" style="display:block;text-decoration:none;color:inherit;border:1px solid var(--card-border-color, #ddd);border-radius:12px;overflow:hidden;background:var(--card-bg, transparent)">
    <img src="/assets/img/projects/bottleneck-sim/card.png" alt="" style="display:block;width:100%;aspect-ratio:16/9;object-fit:cover;margin:0">
    <span style="display:flex;align-items:center;gap:10px;padding:10px 12px">
      <img src="/assets/img/projects/bottleneck-sim/icon.svg" alt="" style="width:36px;height:36px;flex:none;margin:0">
      <span style="display:flex;flex-direction:column;line-height:1.25"><strong>Bottleneck Simulator</strong><small style="opacity:.75">Watch a process choke</small></span>
    </span>
  </a>
</div>

## Desktop apps for Linux

I run Arch Linux with Hyprland, and the desktop tools I missed from other
platforms I ended up writing myself, in GTK 4 and libadwaita so they feel
native on GNOME-style desktops.

### <img src="/assets/img/projects/snip-pin/icon.svg" width="36" style="vertical-align:middle" alt=""> snip-pin {#snip-pin}

![snip-pin: a region is selected on screen and stays pinned above everything as a floating window](snip-pin/card.png){: width="800" }
_Pick a region, a window or an element inside a window, and the screenshot stays exactly where it was taken._

A screenshot tool for Hyprland in the style of Snipaste. Press a key, pick a
region, and the snip floats above everything at its original position: drag
it, zoom it, fade it, annotate it, copy or save it. It snaps to windows and
to the rectangles inside them, keeps a history, and all pins share one
process so a second pin appears in about 50 ms.
[Source on GitHub](https://github.com/felsenuboot/snip-pin).

### <img src="/assets/img/projects/tango/icon.svg" width="36" style="vertical-align:middle" alt=""> Tango 単語 {#tango}

![Tango: a search sidebar and an entry page with the kanji, its stroke order and the senses](tango/card.png){: width="800" }
_A search on the left, the entry with kanji, stroke order and senses on the right._

An offline Japanese dictionary for GNOME, written in Rust. JMdict and
Wadoku side by side, English and German, kanji with stroke order from
KanjiVG, pitch accent, example sentences, JLPT levels, word lists with Anki
export, and a WaniKani integration that marks what you already know. The
search is the one a Jisho user expects, a few milliseconds and offline.

### <img src="/assets/img/projects/den-mail/icon.svg" width="36" style="vertical-align:middle" alt=""> Den Mail {#den-mail}

![Den Mail: a three-pane mail window, the letter pulled out of its envelope in the reading pane](den-mail/card.png){: width="800" }
_Folders, the message list, and the letter out of its envelope._

A Fastmail client for GNOME that talks JMAP directly and keeps a local
cache, so it opens at once, works offline and follows changes by push.
Labels, undo for everything including sending, send later, a screener for
first-time senders, local categories that learn from corrections, rules,
Masked Email, and a lock screen.
[Source on GitHub](https://github.com/felsenuboot/den-mail).

### <img src="/assets/img/projects/yubioath-gtk/icon.svg" width="36" style="vertical-align:middle" alt=""> YubiOath {#yubioath-gtk}

![YubiOath: a list of accounts, one row lit by the YubiKey plugged into the window](yubioath-gtk/card.png){: width="800" }
_The accounts on the key, one row lit by the key itself._

The one-time passwords stored on a YubiKey, in a small GTK 4 window. A
Linux-native replacement for the OTP part of Yubico Authenticator: codes with
a countdown ring, click to copy, favourites, issuer logos, QR import, and a
tray icon that copies a code without opening the window.
[Source on GitHub](https://github.com/felsenuboot/yubioath-gtk).

### <img src="/assets/img/projects/knx-panel/icon.svg" width="36" style="vertical-align:middle" alt=""> Control-9 Wandpanel {#knx-panel}

![Control-9 Wandpanel: a house with four rooms, one of them lit and wired to a tile on the wall panel](knx-panel/card.png){: width="800" }
_A room in the house, wired to its tile on the panel._

A wall panel UI for a Gira Control 9 from 2008: an 800×480 touch screen
running Windows XP Embedded and a Firefox 68 core, which cannot scroll and
cannot decode H.264. A Python server reads Home Assistant and serves one
HTML page of tiles: rooms and zones, lights and blinds, solar, wallbox, pool,
weather with official warnings, the entrance camera, and a screensaver with
the clock. The layout is drawn on the desktop in a configurator and deployed
to the wall within a minute of a push.

## Web apps

### <img src="/assets/img/projects/color-combinator/icon.svg" width="36" style="vertical-align:middle" alt=""> Color Combinator {#color-combinator}

![Color Combinator: a picked colour on the left, its nearest match in Wada's palette and the companion colours on the right](color-combinator/card.png){: width="800" }
_Pick a colour, find its nearest match in the book, see what Wada paired it with._

Sanzo Wada's *A Dictionary of Color Combinations* (配色事典, 1933) as a
companion finder: 159 colours, 348 combinations and the 72 plates of the
Seasons volume. Paste a hex or sample a colour from a photo, and the app
finds its nearest match in the palette and every colour Wada paired it with,
ranked by how often they appear together and traceable to the plate. The
interface is built from the book's own colours.

### <img src="/assets/img/projects/civic-digital/icon.svg" width="36" style="vertical-align:middle" alt=""> Civic Digital {#civic-digital}

![Civic Digital: one page of cards, one per data source, with a map pin dropped on it](civic-digital/card.png){: width="800" }
_One place, one page: weather, departures, water level, air, waste, council._

The most useful public data for one place on one page: weather and official
warnings, live departures, water levels, air quality, the waste calendar,
schools and holidays, the city council. All from open data, fetched
server-side, keyless, failing soft per card. It began as
[Digital.Herdecke](https://github.com/felsenuboot/herdecke-digital) for my
home town, gained a [Dortmund](https://github.com/felsenuboot/dortmund-digital)
sister, and is now one codebase with six deployments, five of them in Japan
(神戸, 大阪, 東京, 関西, 関東), in three languages, on the KERN design system of
the German public administration.

## Research and simulation

### <img src="/assets/img/projects/cultural-distances/icon.svg" width="36" style="vertical-align:middle" alt=""> Cultural Distances {#cultural-distances}

![Cultural Distances: two countries as markers on six dimension tracks, the gap between them drawn in red on each](cultural-distances/card.png){: width="800" }
_Two countries, six dimensions, and the distance between them on each._

A terminal tool from my master's thesis on cultural distance and
overpayment in cross-border M&A. It turns Hofstede's six dimensions and Erin
Meyer's eight Culture Map scales into a distance between every pair of
countries, then shows the result as a network graph, as clusters, or as box
plots with the pairs you care about highlighted.
[Source on GitHub](https://github.com/felsenuboot/Cultural_Distances).

### <img src="/assets/img/projects/bottleneck-sim/icon.svg" width="36" style="vertical-align:middle" alt=""> Bottleneck Simulator {#bottleneck-sim}

![Bottleneck Simulator: two chambers joined by a glowing neck, items crowding in front of it and trickling out behind](bottleneck-sim/card.png){: width="800" }
_Items crowd in front of the neck and trickle out behind it._

A browser simulation of a process line, told through the population
bottleneck metaphor: items flow through wide chambers joined by narrow
necks, and you watch where the queue forms, what the throughput settles at,
and what changes when the neck is widened. Built for explaining on a
projector, with before-and-after comparison, a presentation mode and export
as video or GIF.

## Where this goes

The posts for the individual projects are next, and the cards will show up
on a projects page. If one of these is useful to you, the public ones take
issues and pull requests; the private ones will open up once they are ready.
