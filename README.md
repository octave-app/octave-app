# README – octave-app

[Octave.app](https://octave-app.org) is a native Mac app distribution of [GNU Octave](https://octave.org/). See the [Octave.app web site](https://octave-app.org) for info.

This octave-app repo hosts the releases of Octave.app (in [its GitHub Releases](https://github.com/octave-app/octave-app/releases) section), tracks Octave.app bugs, and related things.

You can download Octave.app from [our Releases page](https://github.com/octave-app/octave-app/releases).

Bugs in Octave.app can be reported in this octave-app repo, in the [octave-app Issues tracker](https://github.com/octave-app/octave-app/issues).

To use GitHub Notifications to be notified of new Octave.app releases, subscribe to [Issue #1 "Announcements"](https://github.com/octave-app/octave-app/issues/1), or [Issue #289 "Dev News"](https://github.com/octave-app/octave-app/issues/289) for betas and prereleases.

This isn't the repo for [GNU Octave](https://octave.org/) itself (aka "core Octave"). For help with regular GNU Octave (as opposed to the special Octave.app packaging of it), see the [GNU Octave Discourse forum](https://octave.discourse.group/).

## Related repos and sites

The `bundle_octave` tool used to create these releases is over in the [octave-app-bundler repo](https://github.com/octave-app/octave-app-bundler).

The custom Homebrew formulae used to build Octave.app are found in the octave-app/octave-app Tap, hosted in the [homebrew-octave-app repo](https://github.com/octave-app/homebrew-octave-app).

The [octave-app.org web site](https://octave-app.org) source is found in the [octave-app.github.io repo](https://github.com/octave-app/octave-app.github.io), and hosted on GitHub Pages.

All these live under the umbrella of the [octave-app GitHub organization](https://github.com/octave-app).

The `create-dmg` tool used in the octave-app-bundler build process is found in the [create-dmg repo](https://github.com/create-dmg/create-dmg) under the separate create-dmg GitHub organization. (The old octave-app/create-dmg repo is an obsolete project fork of that; our customizations were upstreamd around 2021 and now we just use the regular create-dmg instead of our custom variant.)
