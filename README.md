# Highfield Road Uniting Church — AV Documentation

Operating and support documentation for the audio, video, livestream and
presentation system at **Highfield Road Uniting Church**, built with
[MkDocs Material](https://squidfunk.github.io/mkdocs-material/).

The documentation is written for:

- **Volunteer operators** (assumed non-technical, possibly 70+) running the
  Sunday 9:30am service.
- **Future AI-assisted support** using Retrieval Augmented Generation (RAG).
- **Long-term maintenance** by Mills IT.
- **Training** new operators and **reducing support calls**.

## Quick links (once built)

- **Home / start here:** `docs/index.md`
- **Sunday Startup:** `docs/quick-start/sunday-startup.md`
- **Running a Service:** `docs/quick-start/service-operation.md`
- **Sunday Shutdown:** `docs/quick-start/sunday-shutdown.md`
- **Troubleshooting:** `docs/troubleshooting/`
- **Equipment list (authoritative):** `docs/system-design/equipment-list.md`

## Building locally

```bash
# 1. (Optional) create a virtual environment
python3 -m venv .venv && source .venv/bin/activate

# 2. Install dependencies
pip install -r requirements.txt

# 3. Live preview at http://127.0.0.1:8000
mkdocs serve

# 4. Build static site into ./site
mkdocs build
```

## Repository structure

```
mkdocs.yml              # Site configuration and navigation
docs/
  index.md              # Home page
  quick-start/          # Startup, running a service, shutdown
  audio/                # Mixer, microphones, foyer + livestream mixes
  video/                # RodeCaster, cameras, PTZ controller
  presentation/         # PowerPoint, StreamDeck
  displays/             # TV distribution, Bluestream matrix
  troubleshooting/      # Common problems, step-by-step
  system-design/        # Equipment list, signal flow, network
  maintenance/          # Batteries, cleaning, regular checks
  training/             # Volunteer training path, glossary
  assets/               # Images / screenshots (placeholders noted in pages)
```

## Conventions (for editors and AI assistants)

- Use the **exact equipment names** from
  [`docs/system-design/equipment-list.md`](docs/system-design/equipment-list.md).
- Practical operation first, technical detail second.
- Simple language; explain what a control does **before** how to use it.
- Use admonitions for callouts: `!!! tip`, `!!! note`, `!!! warning`,
  `!!! danger`.
- Screenshot placeholders are marked with `📷 *Screenshot placeholder: ...*` —
  replace with real images placed under `docs/assets/`.

## TODO — open items to confirm

Things to verify on site and then update in the docs. Tick off as completed.

### Cameras

- [ ] **Confirm how the cameras are turned on and off.**
      The **AVKANS Joy Pro Controller** (PTZ controller) can turn the cameras
      **off**, but it is **not confirmed** whether it can turn them back **on**
      again. Establish the correct on/off method for both **Camera 1
      (RoboShot HDMI 12)** and **Camera 2 (AVKANS 20X PTZ)**, then:
    - Add a camera power-on step to `docs/quick-start/sunday-startup.md`
      (currently flagged in **Step 7**), and a matching power-off step to
      `docs/quick-start/sunday-shutdown.md`.
    - Update the `*[Mills IT to confirm]*` note in Startup Step 7.
    - If the cameras are simply **always-on** (e.g. powered over the network),
      document that instead and remove the flag.

### Site-specific details to fill in

Several pages contain `*[add ...]*` / `*[Mills IT to confirm]*` placeholders
for site-specific details (IP addresses, stream details, contact numbers,
matrix mappings). Fill these in as the install is finalised:

- [ ] `docs/system-design/equipment-list.md` — QU-5D scene names, YouTube/stream
      details, matrix URL/IP and I/O map, camera IPs/presets, Companion config
      backup location.
- [ ] `docs/system-design/network-overview.md` — router/switch details, static
      IP addresses, wired-vs-wireless, upload speed.
- [ ] `docs/displays/bluestream-matrix.md` — matrix control URL/IP and the
      input/output number map.
- [ ] `docs/maintenance/regular-checks.md` — Mills IT contact details and
      Sunday-morning/emergency contact.
- [ ] `docs/presentation/streamdeck-buttons.md` — confirm the real StreamDeck
      button labels match the documented "typical layout".

### Diagrams and images

- [ ] Replace the draft wiring diagram (`docs/assets/wiring-diagram-v3.png`,
      shown on `docs/system-design/signal-flow.md`) once all connections and
      channels are confirmed; remove the "draft" warning.
- [ ] Replace the `📷 *Screenshot placeholder: ...*` markers with real photos
      placed under `docs/assets/` (see `docs/assets/README.md` for the list).

---

## Maintainer notes

Mills IT maintains this system. The open items above are tracked in the docs
with `*[add ...]*` and `*[Mills IT to confirm]*` markers — search the `docs/`
folder for those strings to find every spot that still needs site-specific
detail.

---

Maintained by **Mills IT**. Church website:
<https://highfieldroadcanterburyuc.org.au/>
