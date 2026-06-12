# Allen & Heath Qu-5D Church Mixer Setup Guide

## Overview

This mixer configuration is designed for:

* Simple volunteer operation
* Separate auditorium, foyer and livestream feeds
* Choir and organ microphones excluded from the auditorium PA
* Improved speech intelligibility
* Reduced feedback risk
* Easy operation from a single fader layer

---

# Channel Layout

| Channel   | Source                  |
| --------- | ----------------------- |
| Ch 1      | Lectern Microphone      |
| Ch 2      | Wireless Handheld 1     |
| Ch 3      | Wireless Handheld 2     |
| Ch 4      | Wireless Headset        |
| Ch 5      | Pulpit Microphone       |
| Ch 6      | Choir Microphone Left   |
| Ch 7      | Choir Microphone Right  |
| Ch 8/9    | Media Playback (Stereo) |
| Remaining | Spare musician inputs   |

---

# Output Layout

| Output     | Purpose       |
| ---------- | ------------- |
| LR         | Auditorium PA |
| Matrix 1-2 | Livestream    |
| Matrix 3-4 | Foyer         |

---

# Choir / Organ Routing

The choir microphones should never be heard through the main auditorium PA.

### Create Stereo Group

Setup → Mixer Config

Configure:

```text
Group 1-2 = Stereo Group
Name = Choir/Organ
```

### Assign Choir Microphones

For each choir microphone:

```text
Assign to Group 1-2
Remove from LR
```

Signal flow:

```text
Choir Mic 1
Choir Mic 2
        ↓
   Group 1-2
        ↓
Livestream Matrix
Foyer Matrix (optional)
```

---

# Livestream Matrix Setup

Create Matrix 1-2 as stereo.

Send:

```text
LR → Matrix 1-2 = 0dB
Group 1-2 → Matrix 1-2 = -5dB (starting point)
```

Adjust choir level during rehearsal.

---

# Foyer Matrix Setup

Create Matrix 3-4 as stereo.

Send:

```text
LR → Matrix 3-4 = 0dB
Group 1-2 → Matrix 3-4 = Optional
```

Suggested starting level:

```text
Group 1-2 → Matrix 3-4 = -10dB
```

---

# Output Patching

Suggested patching:

| Physical Output | Source           |
| --------------- | ---------------- |
| XLR 1           | LR Left          |
| XLR 2           | LR Right         |
| XLR 3           | Livestream Left  |
| XLR 4           | Livestream Right |
| XLR 5           | Foyer Left       |
| XLR 6           | Foyer Right      |

Connections:

```text
XLR 1-2 → Main PA
XLR 3-4 → RodeCaster Video
XLR 5-6 → Foyer Amplifier
```

---

# Matrix Processing

## Livestream Matrix

Add bus compression:

```text
Threshold: -6dB
Ratio: 4:1
Attack: 10ms
Release: 200ms
```

Add limiter:

```text
Threshold: -1dB
```

Purpose:

* Prevent livestream clipping
* Improve online listening experience

---

## Foyer Matrix

Apply:

```text
High Pass Filter: 80Hz
Light Limiting
```

Purpose:

* Cleaner foyer audio
* Protect foyer speakers

---

# Automatic Feedback Suppression

Enable AFS on LR.

Recommended settings:

```text
12 Fixed Filters
12 Live Filters
Mode: Speech/Music
```

Procedure:

1. Turn auditorium PA to normal operating level.
2. Slowly increase gain until ringing occurs.
3. Allow AFS to capture filters.
4. Repeat until all fixed filters are assigned.
5. Save scene.

Leave live filters active during services.

---

# Automatic Mic Mixer

Enable AMM.

Add:

```text
Lectern
Pulpit
Wireless Headset
Wireless Handheld 1
Wireless Handheld 2
```

Do NOT add:

```text
Choir microphones
Media playback
Musicians
Organ microphones
```

Suggested settings:

```text
NOM Attenuation = 3dB
```

Priority:

```text
Wireless Headset = High
Lectern = Medium
Pulpit = Medium
Handheld 1 = Medium
Handheld 2 = Medium
```

Benefits:

* Reduced room noise
* Reduced feedback risk
* Easier volunteer mixing

---

# Volunteer Layer Layout

Configure Layer 1:

| Fader | Source            |
| ----- | ----------------- |
| 1     | Lectern           |
| 2     | Pulpit            |
| 3     | Wireless HH1      |
| 4     | Wireless HH2      |
| 5     | Wireless Headset  |
| 6     | Media Left        |
| 7     | Media Right       |
| 8     | Spare             |
| 9     | Spare             |
| 10    | Spare Musician    |
| 11    | Spare Musician    |
| 12    | Spare Musician    |
| 13    | Choir Group Left  |
| 14    | Choir Group Right |
| 15    | Livestream Matrix |
| 16    | Foyer Matrix      |

---

# Colour Coding

| Type              | Colour |
| ----------------- | ------ |
| Speech Mics       | Blue   |
| Playback          | Green  |
| Choir Group       | Purple |
| Livestream Matrix | Red    |
| Foyer Matrix      | Orange |

---

# Volunteer Operating Notes

Adjust regularly:

```text
Lectern
Pulpit
Wireless microphones
Media playback
```

Adjust occasionally:

```text
Choir/Organ Group
```

Adjust rarely:

```text
Livestream Matrix
Foyer Matrix
```

Normal operating position:

```text
0dB
```

If online viewers report low audio:

```text
Increase Livestream Matrix slightly
```

If foyer volume is excessive:

```text
Reduce Foyer Matrix slightly
```

If choir is too loud online:

```text
Reduce Choir/Organ Group
```

The operator should normally remain on Layer 1 throughout the service.
