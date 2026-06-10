# Livestream Mix

The people watching on **YouTube** hear a **separate sound mix** from the
people in the room. This page explains how that livestream audio is created
and how to fix it when online viewers can't hear properly.

!!! tip "Key fact"
    The livestream uses a **dedicated matrix mix** from the QU-5D. That mix is
    sent to the **RodeCaster Video**, which combines it with the cameras and
    streams it to YouTube. The room speakers are **not** part of this mix.

---

## How the livestream sound is built

```mermaid
flowchart LR
    QU[QU-5D Mixer] -->|Livestream Matrix Mix| RCV[RodeCaster Video]
    RCV -->|Audio + Cameras| YT[YouTube Livestream]
```

- The QU-5D creates a **livestream matrix mix** — its own balance of the
  microphones and music.
- That audio is sent to the **RodeCaster Video**.
- The RodeCaster Video joins the audio to the camera pictures and streams the
  result to **YouTube**.

---

## Why online viewers need their own mix

The room and the livestream are very different listening situations:

- In the **room**, people hear the actual voices in the air plus the speakers.
- **Online**, viewers hear **only** what is in the livestream mix. If a
  microphone is not added to the livestream mix, online viewers hear nothing
  from it — even though the room hears it fine.

!!! note "This explains the most common livestream complaint"
    "We could hear it in church but not online" almost always means a
    microphone (or the music) was **not in the livestream matrix mix**.

---

## Everyday operation

For a normal Sunday the livestream mix is already set up. Your routine jobs:

1. Make sure the **RodeCaster Video** is on (see
   [RodeCaster Video](../video/rodecaster-video.md)).
2. After starting the stream, **listen to the YouTube stream** on a phone or
   the PC to confirm the audio is present and clear.

---

## Checking the livestream audio is going out

1. On the **RodeCaster Video**, check the **audio meters** are moving when
   someone speaks.
2. On a phone, open the **YouTube** stream and listen (use headphones or keep
   the volume low to avoid feedback in the room).

!!! warning "Avoid feedback when monitoring"
    If you listen to the YouTube stream on a loud phone near the microphones,
    it can cause feedback. Use headphones or a low volume.

---

## Why is there no livestream audio?

Work through these in order:

| Check | What to do |
|-------|-----------|
| Are the **microphone faders up** on the QU-5D? | Raise them — if the room can't hear either, fix that first. |
| Is the **livestream matrix master** up and un-muted? | Raise / un-mute it on the QU-5D. |
| Are the **RodeCaster audio meters** moving? | If not, the audio cable from QU-5D to RodeCaster may be the issue — note for Mills IT. |
| Is the stream actually **live**? | See [RodeCaster Video](../video/rodecaster-video.md). |
| Specific mic missing online only | That mic is not in the livestream matrix — raise it in the **livestream matrix**, not just the main mix. |

➡️ Full guide: [No Livestream Audio](../troubleshooting/no-livestream-audio.md).

---

## Adjusting a microphone for the livestream only

If a microphone is fine in the room but too quiet online (or missing):

1. On the QU-5D, select the **livestream matrix** mix.
2. Find that microphone's **send** to the matrix.
3. Raise it to a sensible level.

!!! warning "Ask before re-balancing if unsure"
    Changing matrix sends affects every future service. If you are not
    confident, raise the main faders, note the problem, and ask Mills IT to
    set the livestream balance correctly.

---

## Related pages

- [Audio Overview](overview.md)
- [QU-5D Mixer](qu5d-overview.md)
- [RodeCaster Video](../video/rodecaster-video.md)
- [No Livestream Audio](../troubleshooting/no-livestream-audio.md)
