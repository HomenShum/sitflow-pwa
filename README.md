# SitFlow PWA preview

This repository stores the SitFlow web preview as checked-in static files. The reviewed tree contains HTML route artifacts and an `_expo/` output directory, rather than the application's editable source project.

## Start here

- [index.html](index.html): exported web entry file.
- [calendar.html](calendar.html), [clients.html](clients.html) and [agent.html](agent.html): other exported route files.
- [Pages workflow](.github/workflows/pages.yml): declared publication path.

At the reviewed commit, there is no package manifest, lockfile or project-defined install/dev/build/test command. Application development or regenerating this export requires the original app source and its setup instructions; their location and commands were not established by this review. No package installation is needed merely to inspect this repository's files.

## Publication and verification scope

The workflow declares publication on a push to `main` or manual dispatch. It checks out the repository, uploads the repository root as a Pages artifact and invokes deployment to GitHub Pages. It declares no application install, build or test step. A documentation merge to `main` also matches that push trigger; actual execution depends on repository Actions/Pages configuration.

This handoff is bound to source commit [`c3eefef`](https://github.com/HomenShum/sitflow-pwa/commit/c3eefef560c4822913ab764b5f8f7c2f298a2fba). Only Git tree metadata and the workflow source were inspected. Generated page/bundle/media bodies, the current Pages state and live URL, rendering, authentication, offline/PWA behavior and backend connectivity were not verified. The repository name and exported routes are not evidence that those flows currently work.

[README documentation history](CHANGELOG/docs/readme.md)
