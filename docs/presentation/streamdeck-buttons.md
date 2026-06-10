# StreamDeck Buttons

The **StreamDeck XL** is the panel of labelled buttons on the operator desk.
Each button lights up and has a label. Pressing a button runs a job for you —
switching a camera, starting the stream, or moving to a saved camera position
— so you do not have to operate the cameras, RodeCaster or PC directly.

The StreamDeck is powered by software called **Bitfocus Companion**, which runs
on the presentation PC (the NUC).

📷 *Screenshot placeholder: the StreamDeck XL with all buttons labelled.*

---

## What the StreamDeck is (and isn't)

- It **is** a set of shortcuts. One button can do several steps at once.
- It is **not** a separate computer. It only works when the **NUC and
  Companion are running**. If the NUC is off, the buttons do nothing.

!!! note "Why we use it"
    Volunteers should not have to learn the RodeCaster, the cameras and the PC
    separately. The StreamDeck turns the common jobs into single, labelled
    button presses.

---

## Typical button layout

!!! warning "Labels are the source of truth"
    The exact buttons can change as the system is improved. **Always read the
    label on the button.** The table below is a typical layout — update this
    page if Companion is changed.

| Button (typical label) | What it does |
|------------------------|--------------|
| **Start Stream** | Begins the YouTube livestream on the RodeCaster |
| **Stop Stream** | Ends the livestream |
| **Camera 1** | Shows the wide camera (RoboShot) on the livestream |
| **Camera 2** | Shows the close-up camera (AVKANS) on the livestream |
| **Cam 2 → Lectern** | Moves Camera 2 to the saved lectern close-up |
| **Cam 2 → Pulpit** | Moves Camera 2 to the saved pulpit close-up |
| **Wide Front** | Moves Camera 1 to the saved wide shot |
| **Next Slide** | Advances the PowerPoint |
| **Previous Slide** | Goes back one PowerPoint slide |
| **Holding Slide** | Shows the welcome / holding screen |

---

## How to use the buttons

### Start the livestream
Press **Start Stream**. Wait for the live indicator, then check YouTube. See
[RodeCaster Video](../video/rodecaster-video.md).

### Switch which camera is shown
Press **Camera 1** (wide) or **Camera 2** (close-up). The picture changes
smoothly. See [Camera Operation](../video/camera-operation.md).

### Send a camera to a saved position (preset)
Press a preset button such as **Cam 2 → Lectern**. The camera moves itself to
that spot.

!!! warning "Move the off-air camera, then switch"
    If you send the **live** camera to a new position, viewers see it move.
    Send the **off-air** camera to its preset first, then switch the livestream
    to it. See [Camera Operation](../video/camera-operation.md#dont-switch-while-moving).

### Advance the slides
Press **Next Slide** / **Previous Slide**. See
[PowerPoint Operation](powerpoint-operation.md).

### Stop the livestream
Press **Stop Stream** at the end of the service. See
[Sunday Shutdown](../quick-start/sunday-shutdown.md).

---

## If a button doesn't work

| Symptom | Likely cause | Fix |
|---------|--------------|-----|
| **No buttons lit at all** | NUC off, or StreamDeck unplugged | Turn on the NUC; check the USB cable |
| Buttons lit but nothing happens | Companion not running, or device offline | Restart Companion on the NUC, or restart the NUC |
| Camera button works, preset doesn't | Camera moved/renamed, or preset changed | Use the joystick ([PTZ Controller](../video/ptz-controller.md)); note for Mills IT |
| Stream button does nothing | RodeCaster off or not connected | Check the RodeCaster ([RodeCaster Video](../video/rodecaster-video.md)) |

!!! tip "The all-purpose first fix"
    If the StreamDeck is behaving oddly, the safest fix is to **restart the
    NUC** (shut down and power back on), which restarts Companion. Do this
    **before** a service, not during, if you can.

---

## For maintainers (Mills IT)

- Companion runs on the **NUC**; the StreamDeck XL connects to it by USB.
- Button actions control the **RodeCaster Video**, the **cameras** and
  **PowerPoint**.
- Keep the **typical button layout** table above in step with the live
  Companion configuration so this page stays accurate for RAG and training.

---

## Related pages

- [RodeCaster Video](../video/rodecaster-video.md)
- [Camera Operation](../video/camera-operation.md)
- [PowerPoint Operation](powerpoint-operation.md)
