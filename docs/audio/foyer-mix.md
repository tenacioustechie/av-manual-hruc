# Foyer Mix

The **foyer** has its own speakers so people in the foyer can hear the service.
This page explains how the foyer sound works and how to fix it if it goes
quiet.

!!! tip "Key fact"
    The foyer uses a **dedicated matrix mix** from the QU-5D, sent to the
    **foyer amplifier**, which drives the **foyer speakers**. It is **separate**
    from the church speakers — so the foyer can be quiet even when the church
    sounds fine.

---

## How the foyer sound is built

```mermaid
flowchart LR
    QU[QU-5D Mixer] -->|Foyer Matrix Mix| AMP[Foyer Amplifier]
    AMP --> SPK[Foyer Speakers]
```

- The QU-5D creates a **foyer matrix mix** — its own balance of the
  microphones.
- That mix is sent to the **foyer amplifier** (the foyer speakers are not
  powered on their own, so they need this amplifier).
- The amplifier drives the **foyer speakers**.

!!! note "Why a separate mix?"
    The foyer is a different space with different needs. A separate mix lets
    us send mainly **voices** to the foyer at a comfortable level, without the
    full musical volume of the main room.

---

## Everyday operation

For a normal Sunday you usually do **not** need to touch the foyer mix — it is
set up to follow the service automatically once the amplifier is on.

Your only routine job is:

1. At startup, make sure the **foyer amplifier is switched on**.
2. During the service, if asked, check the foyer level sounds comfortable.

➡️ Startup step: [Sunday Startup — Step 6](../quick-start/sunday-startup.md#step-6-turn-on-the-foyer-amplifier).

---

## Adjusting the foyer level (if needed)

If the foyer is too quiet or too loud, the level is controlled by the **foyer
matrix master** on the QU-5D:

1. On the QU-5D, select the **foyer matrix** (it is labelled).
2. Raise or lower its **master fader** a little.
3. Check the foyer again.

!!! warning "Make small changes"
    Adjust in small steps and listen. Big jumps can make the foyer suddenly
    too loud.

---

## Why is the foyer audio missing?

Work through these in order:

| Check | What to do |
|-------|-----------|
| Is the **foyer amplifier on**? | Switch it on. This is the most common cause. |
| Is the **foyer matrix master** up on the QU-5D? | Raise it to its normal mark. |
| Is the matrix **muted**? | Un-mute it. |
| Do the **microphones work in the room**? | If not, fix that first — see [No Sound](../troubleshooting/no-sound.md). |
| Still nothing? | The foyer speaker cabling or amplifier may have a fault — note it for Mills IT. |

➡️ Full guide: there is no separate foyer troubleshooting page — use this
section and [No Sound](../troubleshooting/no-sound.md).

---

## Related pages

- [Audio Overview](overview.md)
- [QU-5D Mixer](qu5d-overview.md)
- [Livestream Mix](livestream-mix.md)
