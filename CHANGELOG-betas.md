## CHANGELOG for betas and special releases

## Special Installation Instructions - REQUIRED!

TL;DR: Use `xattr -c` to un-quarantine the DMG before opening it.

After downloading the DMG, before opening it (double-clicking it) to do the installation, you must first "un-quarantine" it. Open Terminal and run `xattr -c ~/Downloads/Octave-*.dmg`. Then you can double-click the DMG file and proceed to install it as usual. If you don't do this extra `xattr -c` step, it will probably just give you an "app is damaged" error instead of launching when you try to run it from /Applications. Sorry; working on fixing this, but not super hopeful. See [#244 – App "damaged" for GitHub downloads](https://github.com/octave-app/octave-app/issues/244).


## 9.2 beta2

Since 9.2.0 beta1:

* All the changes in 9.1.0 beta4 and maybe beta3

## 9.1 beta5

Since 9.1.0 beta4:

* Use 2-part "x.y" version label like "9.1", not "x.y.z", for ".0" releases.
* Have `pkg` custom install location use release suffixes like "_beta1".
* Add gnu-units package, to support miscellaneous OF package.
* Bump some deps.
* App launcher script refinements
  * Remove use of `logger`, quote filenames in open action, remove gnuplot stuff.
* Fix `diagnostic_dump` syntax errors from GNU Octave code style conversion.
  * The function was completely broken before this.
* `diagnostic_dump` enhancements
  * Handle running from non-octapp installation, show full root path.
  * Show Xcode & CLT versions, expand displayed mkoctfile vars.
  * Have output file name include date, host, octapp version, etc., add options.

Since 9.1.0 beta3:

* Qt 6 instead of Qt 5.
* Fix some linkage issues with spuriously-relocatable bottles.
* Built on macOS 12 instead of 14, for better compatibility across OS versions.
* Built on isolated "clean" build boxes (without system Homebrew packages etc.)
* Add plain `octave` command link to the internal `usr/bin`.

Since 9.1.0 beta2:

* Add ipopt package, to support building mexIPOPT.

Since 9.1.0 beta1:

* Fix app size bloat due to llvm/rust/etc inclusion.
* Bump dependency versions.
* Move `octave_app_diagnostic_dump` function to namespaced `octapp.diagnostic_dump`.
* Probably something else I forgot.

Since 8.x:

* Octave 9.1.0.
* Drop librsvg package, to reduce app size.
