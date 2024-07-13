# Octave.app CHANGELOG

This is the changelog for Octave.app, the native Mac app bundle of GNU Octave.

This has info about the user-facing changes in the app itself. It doesn't include info about developer-facing changes in `bundle_octapp` and the other build tools used to create Octave.app; see the [octave-app-bundler repo's](https://github.com/octave-app/octave-app-bundler) CHANGELOG.md for that.

You can also subscribe to the [#1 - Octave.app Announcements](https://github.com/octave-app/octave-app/issues/1) and/or [#289 - Octave.app Dev News](https://github.com/octave-app/octave-app/issues/289) issues on our GitHub repo to receive notifications of when these changes hit releases of Octave.app.

This changelog file was added late in the project's history, in 2023, and there are years of Octave.app history before that which are not captured here.

The releases in this file are arranged in chronological order. This means some version numbers may be out of order, because we sometimes do "update" releases to older-Octave-version releases, and sometimes Octave itself makes patch releases to older minor or major Octave versions. This file is human-readable, not intended to be machine-parseable, and items for previous releases may be retroactively reformatted or revised. The diffs or commit history to this file do not mean anything in particular.

## 8.4 update 1 (unreleased)

* Still Octave 8.4.0.
* Fix inflated app size due to accidentally-retained build-time-only dependencies like versioned llvm package. [#277](https://github.com/octave-app/octave-app/issues/277)
* Built on macOS 12 instead of macOS 14 for greater compatibility.
* Move `octave_app_diagnostic_dump` function to namespaced `octapp.diagnostic_dump`.
* Fix `octapp.diagnostic_dump` breakage due to syntax errors from previous code style update. [#285](https://github.com/octave-app/octave-app/issues/285)
* Expand and fix up `octapp.diagnostic_dump`. [#286](https://github.com/octave-app/octave-app/issues/286)
* Switch to two-part "x.y" instead of "x.y.z" version labels when the ".z" part is ".0". [#287](https://github.com/octave-app/octave-app/issues/287)

(These are mostly backported changes from 9.1.)

## 9.2 (unreleased)

* Octave 9.2.0. [#288](https://github.com/octave-app/octave-app/issues/288)

## 9.1 (unreleased)

* Octave 9.1.0. [#270](https://github.com/octave-app/octave-app/issues/270)
* Use Qt 6 instead of Qt 5. [#262](https://github.com/octave-app/octave-app/issues/262)
* Use 2-part "x.y" version label like "9.1", not "x.y.z", for ".0" releases. [#287](https://github.com/octave-app/octave-app/issues/287)
* Built on macOS 12 instead of 14, for better compatibility across OS versions.
* Fix inflated app size due to accidentally-retained build-time-only dependencies like versioned llvm package. [#277](https://github.com/octave-app/octave-app/issues/277)
* Have `pkg` custom install location use release suffixes like "_beta1".
* Fix some DLL linkage issues with "spuriously relocatable" bottles. [#274](https://github.com/octave-app/octave-app/issues/274)
* App launcher script refinements
  * Remove use of `logger`, quote filenames in open action, remove gnuplot stuff.
* `diagnostic_dump` changes
  * Move `octave_app_diagnostic_dump` function to namespaced `octapp.diagnostic_dump`.
  * Fix `diagnostic_dump` syntax errors from GNU Octave code style conversion. [#285](https://github.com/octave-app/octave-app/issues/285)
    * The function was completely broken before this.
  * `diagnostic_dump` enhancements [#286](https://github.com/octave-app/octave-app/issues/286)
    * Handle running from non-octapp installation, show full root path.
    * Show Xcode & CLT versions, expand displayed mkoctfile vars.
    * Have output file name include date, host, octapp version, etc., add options.
* Add plain `octave` command link to the internal `usr/bin`.
* Bundled package changes
  * Add gnu-units package, to support miscellaneous OF package. [#160](https://github.com/octave-app/octave-app/issues/160)
  * Add ipopt package, to support building mexIPOPT. [#280](https://github.com/octave-app/octave-app/issues/280)
  * Drop librsvg package, to reduce app size.


## 8.4.0 (2024-05-02)

* Octave 8.4.0. [#243](https://github.com/octave-app/octave-app/issues/243)
* First 8.x (or even 7.x) release.
* Drop gnuplot graphics back-end.
* Add native Apple Silicon support, as a separate build and installer. [#205](https://github.com/octave-app/octave-app/issues/205)
* Include netcdf package, for OF packages that need it. [#221](https://github.com/octave-app/octave-app/issues/221)
* Reduce app size by pruning build-time-only dependencies like rust and llvm. [#248](https://github.com/octave-app/octave-app/issues/248)
* Drop Python 3.9 and 3.10 support. [#247](https://github.com/octave-app/octave-app/issues/247)
* Adjust app bundle name, including prerelease indicators in the name.
* Move `octave_app_diagnostic_dump` tool to package-qualified `octapp.diagnostic_dump`.
