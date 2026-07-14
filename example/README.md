# snptx1.github.io/professional/example/

Per-application tailored resume variants. One folder per posting.

## URL pattern

```
https://snptx1.github.io/professional/example/<slug>/
```

where `<slug>` is `<YYYY-MM-DD>__<company>__<role-slug>`, mirroring the run
folder name in the private `snptx-core` scaffolding.

## What lives here

- `example/<slug>/index.html` — the tailored HTML resume
- `example/<slug>/resume.pdf` — the shipped PDF (optional, for direct portal upload)
- `example/<slug>/cover_letter.pdf` — the shipped cover letter (optional)

Nothing under `example/<slug>/` is discoverable from the canonical resume at
the root of this repo. Each URL is only shared with the specific applicant
portal or recruiter.

## Provenance

Each tailored variant is generated from `templates/resume_template.html` in the
private `snptx-core` repo, filled from `templates/profile.yaml` (source of
truth for facts), and only published here after a human `APPROVED` marker
has been recorded in the corresponding `runs/<slug>/` directory.
