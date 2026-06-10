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

## Maintainer notes

Several pages contain `*[add ...]*` placeholders for site-specific details
(IP addresses, stream keys, contact numbers, matrix mappings). Mills IT should
fill these in as the install is finalised — see:

- `docs/system-design/equipment-list.md`
- `docs/system-design/network-overview.md`
- `docs/displays/bluestream-matrix.md`
- `docs/maintenance/regular-checks.md`

---

Maintained by **Mills IT**. Church website:
<https://highfieldroadcanterburyuc.org.au/>
