# Equipment List

A complete, named inventory of the AV system at Highfield Road Uniting Church.
Use the **exact names** in this list throughout the documentation so operators,
maintainers and AI assistants all refer to the same things.

!!! note "For AI assistants and maintainers"
    This is the authoritative equipment reference. Each item lists its role and
    the page that explains how to use it.

---

## Audio

| Equipment | Role | Details page |
|-----------|------|--------------|
| **Allen & Heath QU-5D** | Central audio mixer; creates the main, foyer and livestream mixes | [QU-5D Mixer](../audio/qu5d-overview.md) |
| **JBL SRX812P** (powered speakers) | Main auditorium loudspeakers | [Audio Overview](../audio/overview.md) |
| **Foyer amplifier** | Drives the foyer speakers RedBack 2x125W A4072B | [Foyer Mix](../audio/foyer-mix.md) |
| **Foyer speakers** | Play the foyer mix in the foyer 100v roof disk speakers | [Foyer Mix](../audio/foyer-mix.md) |

### Microphones

| Channel | Microphone | Type | Used for |
|--------:|------------|------|----------|
| 1 | Lectern Sennheiser condenser | Wired | Lectern speaker |
| 2 | Handheld Roving radio microphone | Wireless | Roving / guest |
| 3 | Handheld Elder radio microphone | Wireless | Roving / guest |
| 4 | Headset radio microphone | Wireless | Hands-free leader |
| 5 | Pulpit Sennheiser condenser | Wired | Pulpit speaker |
| — | Stereo pair of Rode M5 condenser | Wired | Choir and organ |

➡️ [Microphone Guide](../audio/microphone-guide.md)

### Audio outputs (mixes)

| Output | Destination |
|--------|-------------|
| Main mix (LR) | JBL SRX812P speakers (auditorium) |
| Foyer matrix mix | Foyer amplifier → foyer speakers |
| Livestream matrix mix | RodeCaster Video → YouTube |

---

## Video

| Equipment | Role | Details page |
|-----------|------|--------------|
| **RodeCaster Video** | Central video switcher and livestream encoder; streams to YouTube | [RodeCaster Video](../video/rodecaster-video.md) |
| **Camera 1 — RoboShot HDMI 12** | PTZ camera, usually the wide shot | [Camera Operation](../video/camera-operation.md) |
| **Camera 2 — AVKANS 20X PTZ Camera Pro** | PTZ camera, usually close-ups (20× zoom) | [Camera Operation](../video/camera-operation.md) |
| **AVKANS Joy Pro Controller** | Joystick to pan/tilt/zoom the cameras by hand | [PTZ Controller](../video/ptz-controller.md) |

---

## Operator control

| Equipment | Role | Details page |
|-----------|------|--------------|
| **StreamDeck XL** | Panel of labelled buttons for common jobs | [StreamDeck Buttons](../presentation/streamdeck-buttons.md) |
| **Bitfocus Companion** | Software (on the NUC) that powers the StreamDeck buttons | [StreamDeck Buttons](../presentation/streamdeck-buttons.md) |

---

## Presentation

| Equipment | Role | Details page |
|-----------|------|--------------|
| **Presentation PC — Mini Windows NUC** | Runs PowerPoint and Companion | [PowerPoint Operation](../presentation/powerpoint-operation.md) |
| **Microsoft PowerPoint** | Shows song words, readings, notices | [PowerPoint Operation](../presentation/powerpoint-operation.md) |

---

## Display distribution

| Equipment | Role | Details page |
|-----------|------|--------------|
| **Bluestream HDMI Matrix** | Routes the PC picture to the various screens (the **picture**) | [Bluestream Matrix](../displays/bluestream-matrix.md) |
| **RTI 7" touch screen controller** | Turns the TVs on/off (the **power**); located just below the PC | [TV Distribution](../displays/tv-distribution.md) |

### Displays

| Screen | Location | Normally shows |
|--------|----------|----------------|
| Front TV Left | Front auditorium, left | PowerPoint slides |
| Front TV Right | Front auditorium, right | PowerPoint slides |
| Rear Confidence Monitor | Faces the speaker | PowerPoint slides |
| Fireplace TV | Fireplace area | Slides (optional) |
| Meeting Room TV | Meeting room | Slides (optional) |

➡️ [TV Distribution](../displays/tv-distribution.md)

### Media sources

| Equipment | Role |
|-----------|------|
| **Apple TV** | HDMI media source (e.g. streamed/online content). Powered by the **top power strip**. |
| **Blu-ray player** | HDMI media source for discs. Powered by the **top power strip**. |

!!! note "Powered by the top power strip"
    The Apple TV and Blu-ray player, together with the **three radio microphone
    receivers**, are switched on/off by the **top power strip** at the back of
    the rack (see [Sunday Startup — Step 7](../quick-start/sunday-startup.md#step-7-turn-on-the-small-devices)).

---

## Streaming

| Item | Detail |
|------|--------|
| Streaming source | **RodeCaster Video** |
| Streaming destination | **YouTube** |
| Service time | **Sunday 9:30am** |
| Church website | <https://highfieldroadcanterburyuc.org.au/> |

---

## Maintainer notes (fill in as known)

Mills IT — record specifics here for long-term maintenance:

- QU-5D scene name(s) used for Sunday: *[add]*
- YouTube channel / stream details location: *[add]*
- Fixed Device IP addresses are listed below in 'Network Details'
- Camera IP addresses and preset numbers: *[add]*
- Companion version and config backup location: *[add]*

➡️ See also [Signal Flow](signal-flow.md) and [Network Overview](network-overview.md).

## Network Details

| Device | IP Address |
| --- | --- |
| PC at Sounddesk | 192.168.1.16 ? |
| QU-5 Mixer | 192.168.1.15 |
| RodeCaster Video | 192.168.1.17 |
| BluStream HDMI Matrix | 192.168.1.3 |
| Camera 1 Roboshot | 192.168.1.4 |
| Camera 2 AVKANS | 192.168.1.25 |
| PTZ Controller AVKANS | 192.168.1.4 |