<p align="center">
  <a href="https://gazeora.github.io">
    <img src="https://gazeora.github.io/assets/logo.png" alt="Gazeora" width="96" height="96">
  </a>
</p>

<h1 align="center">Gazeora</h1>

<p align="center">
  Your PC games, on your phone, in VR.<br>
  <a href="https://gazeora.github.io">Website</a> ·
  <a href="https://gazeora.github.io/download.html">Download</a> ·
  <a href="https://gazeora.github.io/docs.html">Docs</a>
</p>

Gazeora captures a game's frames on a Windows PC as it renders them and streams them live to
any device on your local network. Put your phone in a Cardboard-style VR viewer and the game
shows as a flat screen in front of you, with real depth.

It's free software, under the GNU GPL version 3.

## Repositories

| Repository | What it is |
|---|---|
| [Gazeora](https://github.com/Gazeora/Gazeora) | The Windows launcher and stream server. Captures Direct3D 8 to 12 and OpenGL games, encodes on the GPU as H.264 or H.265, and streams over RTSP, HTTP, UDP or USB. C++17 |
| [Gazeora-Android](https://github.com/Gazeora/Gazeora-Android) | The Android viewer. Finds PCs on the network by itself, plays the stream full screen over Wi-Fi or a USB cable, flat or for a VR viewer, and turns touches into a mouse. Java and C++ |
| [gazeora.github.io](https://github.com/Gazeora/gazeora.github.io) | The website, with downloads for every release and the guides |
| [.github](https://github.com/Gazeora/.github) | Issue forms and the pull request template shared by every repository |

## How it fits together

```
 Windows PC                                              Phone or any device on the LAN
┌───────────────────────────────────────┐   Wi-Fi or   ┌───────────────────────────────┐
│ Game  ──hook──►  Gazeora              │   USB cable  │ Gazeora for Android           │
│                  capture, VR layout,  │═════════════►│  decode, lens correction,     │
│                  H.264 / H.265 encode │◄─────────────│  touch as a mouse             │
└───────────────────────────────────────┘    touches   │ or VLC / ffplay / OBS (RTSP)  │
                                                       └───────────────────────────────┘
```

## Getting started

1. Install Gazeora on the PC: the **x64** release for 64-bit games, the **x86** release for
   32-bit ones. Installers are on the [download page](https://gazeora.github.io/download.html).
2. Install the Android app on the phone, from the same page.
3. Launch a game from Gazeora with **Play with capture**, then open the app. The PC shows up in
   its list by itself.

## Contributing

Bug reports, game compatibility reports, phone reports and pull requests are welcome. Each
repository's `CONTRIBUTING.md` says how. Issues use forms, so pick the one that fits: bug,
crash or freeze, performance, game compatibility or feature request. Questions go to
Discussions, and security problems to private vulnerability reporting.

## License

Copyright (C) 2026 Nithin Aashik. Gazeora is free software under the GNU GPL version 3, with
the additional terms in each repository's `NOTICE`: modified versions keep the attribution
"Gazeora by Nithin Aashik", are marked as modified, and don't use the Gazeora name or logo as
their own ([TRADEMARKS.md](https://github.com/Gazeora/Gazeora/blob/master/TRADEMARKS.md)).
