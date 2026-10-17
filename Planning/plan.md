# Portfolio Website — Plan

## Goal
Static portfolio site hosted on GitHub Pages, showcasing mechatronics projects (CAD, electronics, firmware) for RodLDR.

## Stack
- Jekyll (native GitHub Pages build, no Actions pipeline needed)
- Repo: `RodLDR/portfolio` (project repo, not `username.github.io`)
- Served at: `https://rodldr.github.io/portfolio/`
- No custom domain, no theme dependency — custom minimal layouts in `_layouts/`

## Site structure
```
portfolio/
├── _config.yml
├── Gemfile
├── index.md              # home page, lists all projects
├── about.md               # bio, skills, resume link
├── _projects/             # one file per project (Jekyll collection)
├── _layouts/
│   ├── default.html
│   └── project.html
└── assets/
    ├── css/style.css
    └── images/<project-slug>/
```

## Per-project template sections
1. Summary (1-2 sentences)
2. My role & tools
3. Problem/goal
4. Mechanical (renders, exploded view, drawings) — if applicable
5. Electronics (schematic/PCB) — if applicable
6. Firmware/control (snippet + repo link) — if applicable
7. Results (demo video/GIF)
8. Links (GitHub repo, PDFs)

## Projects tracked (see `project-list.md` for details/status)
1. RobotArm — 4-DOF cobot-style robotic arm
2. RobotRubik — Rubik's cube-solving robot
3. ModularMinitank — modular Arduino shield tank
4. CADPractice: V6 Motor (SolidWorks)
5. CADPractice: Radial Motor (Solid Edge)

## Resource estimate

| Task | Time |
|---|---|
| Jekyll setup + layout/CSS | 4-6 hrs |
| Writing per-project content (5 × ~1-1.5 hrs) | 5-7.5 hrs |
| Producing/organizing missing media (renders, PCB screenshots, trimming videos) | 4-8 hrs |
| About/bio/resume page | 1-2 hrs |
| Testing (mobile view, links, image sizes) + polish | 2-3 hrs |
| **Total** | **~16-26.5 hrs** |

Cost: $0 (GitHub Pages hosting + `*.github.io` subdomain path are free; videos embedded via YouTube instead of stored in repo to avoid the ~1GB soft repo size limit).

## Status
- [x] Repo scaffolded, pushed to GitHub
- [ ] GitHub Pages enabled and first build verified
- [ ] Real content (text, images, links) filled in per project — see `content-checklist.md`
- [ ] About page filled in
- [ ] Final polish / mobile check
