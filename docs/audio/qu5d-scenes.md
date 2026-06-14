# QU-5D Scenes (save & recall)

A **scene** is a saved snapshot of all the mixer settings — every fader level,
mute, routing and EQ. Scenes let you return the desk to a known-good starting
point in seconds, and let you keep a different setup for each kind of event.

There are two things you can do with a scene:

- **Recall** — load a saved scene. **Safe.** This is the everyday job, done at
  startup every Sunday.
- **Save (store)** — capture the current settings into a scene. **Not routine.**
  This *changes the starting point for everyone* who uses the desk after you.

!!! warning "Saving is an admin task — recall is the everyday one"
    For a normal Sunday you only ever **recall**. You **save** a scene only when
    you are deliberately setting a new "normal" — for example after the system
    has been re-tuned, or when preparing a setup for a special event.

    Saving **overwrites** whatever was in that scene slot. Save to the **right
    slot**, and let **Mills IT** know when you change the Sunday scene so the
    backup stays current. See [Regular Checks](../maintenance/regular-checks.md).

📷 *Screenshot placeholder: Scenes screen on the QU-5D touchscreen, with the scene list, Recall and Store buttons labelled.*

---

## Recalling a scene

Use this to get the desk back to a known-good setup.

1. On the QU-5D touchscreen, open **Scenes** *[Mills IT to confirm exact button:
   `Setup` → `Scenes`, or a dedicated `Scenes` key]*.
2. In the list, tap the scene you want (e.g. **Sunday Service**).
3. Press **Recall** and confirm.
4. Check the faders and the **L/R** button have moved/lit to the recalled
   settings. (More on the L/R button:
   [QU-5D Mixer — Master / main fader](qu5d-overview.md#master-main-fader).)

!!! tip "Recall is your reset button"
    If someone has changed the desk and you are not sure what, recalling the
    **Sunday Service** scene is the quickest way back to normal.

---

## Saving / updating the Sunday Service scene

Do this only when you want the **normal Sunday starting point** to change.

**1. Set the desk exactly how you want it to start each Sunday.**

   - Faders at their correct levels.
   - The right channels muted / un-muted.
   - Routing correct (room, foyer matrix, livestream matrix).
   - The **L/R** button **lit** above the master fader, master fader at its mark.

**2. Open the Scenes screen** [`Scenes` Button under touch screen]

**3. Select the existing Sunday slot.** Tap the **Sunday Service** scene in the
   list so it is highlighted. (You are overwriting this slot, not making a new
   one.)

**4. Press Store / Save** *[Mills IT to confirm exact label — `Store` on Qu
   desks]*. Confirm if asked.

**5. Check the name is still "Sunday Service"** and that the slot number matches
   the one recorded in
   [Equipment List → Maintainer notes](../system-design/equipment-list.md#maintainer-notes-fill-in-as-known).

!!! danger "Make sure the right slot is highlighted before you Store"
    **Store writes to whichever scene is selected.** Double-check **Sunday
    Service** is the highlighted one — storing onto the wrong slot will quietly
    replace a different event's setup.

---

## Creating a scene for another event

For a **funeral**, **concert**, **AGM** or similar, make a **new** scene rather
than changing the Sunday one.

1. **Start from a known base.** Recall the **Sunday Service** scene first, so you
   begin from a working setup.
2. **Adjust** the desk for the event (e.g. extra mics for a choir, different
   foyer level).
3. **Set the L/R** button lit and the master fader at its mark, as usual.
4. **Open Scenes**, then tap an **empty / spare slot** — **not** the Sunday slot.
5. **Press Store / Save**, then **name** the scene clearly (see naming below).

!!! warning "Never overwrite the Sunday Service scene for a one-off event"
    Save event setups to their **own** slot. The Sunday scene must always stay
    ready for the next normal service.

### Naming convention

Keep names short and obvious so the next operator can pick the right one:

| Use this kind of name | Example |
|-----------------------|---------|
| Regular service | `Sunday Service` |
| Recurring event type | `Funeral` |
| Recurring event type | `Concert` |
| Recurring event type | `AGM / Meeting` |
| One-off, dated | `Carols 24-12` |

Avoid vague names like `Test`, `New` or `Scene 12`.

---

## Scene list (record what each slot is for)

Keep the actual slot numbers and names recorded so they are not lost. The
master record lives in
[Equipment List → Maintainer notes](../system-design/equipment-list.md#maintainer-notes-fill-in-as-known):

| Slot | Scene name | Used for |
|-----:|------------|----------|
| 1 | Sunday Service | Normal 9:30am service |
| *[add]* | *[add]* | *[add]* |

---

## What a scene does and does not change

!!! note "A scene restores settings, not hardware"
    Recalling a scene sets faders, mutes, routing and EQ. It does **not** turn on
    the speakers, the mixer or any other device, and it does **not** fix a flat
    radio-mic battery or a mic switched off. Those are still part of your
    [Sunday Startup](../quick-start/sunday-startup.md) checks.

---

## Related pages

- [QU-5D Mixer](qu5d-overview.md)
- [Sunday Startup](../quick-start/sunday-startup.md)
- [Equipment List](../system-design/equipment-list.md)
- [Regular Checks](../maintenance/regular-checks.md)
