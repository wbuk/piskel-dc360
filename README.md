# piskel-dc360

Ready-built copies of [Piskel](https://github.com/piskelapp/piskel), the free pixel-art and sprite editor by
Julian Descottes and contributors (Apache License 2.0).

Piskel has not published built releases since 2018, but it is still being developed. Every night the job in
`.github/workflows/build.yml` checks Piskel's `master` branch. When there is a new commit, it builds Piskel with
Piskel's own build (`npm run build`) and publishes the result here as a release:

- the release is named after the time of Piskel's commit (UTC): `vYYYY.MMDD.HHMM`, so a newer one is always higher;
- `piskel-dc360.zip` holds the built editor (`index.html`, `js/`, `css/`, `img/`), Piskel's licence
  (`LICENSE.txt`) and `piskel-build.json` (the commit it was built from).

This repository contains no changes to Piskel. It is used by DC360, which downloads these releases and applies
its own changes on its own server.

To build straight away instead of waiting for the night: **Actions > Build Piskel > Run workflow**.
