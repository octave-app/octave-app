# Octave.app CHANGELOG

This is the changelog for Octave.app, the native Mac app bundle of GNU Octave.

This has info about the user-facing changes in the app itself. It doesn't include developer info about the build tools used to create Octave.app; see the octave-app-bundler repo for that.

## 8.4.0 (unreleased)

* First 8.x (or even 7.x) release.
* Drop gnuplot graphics back-end.
* Add native Apple Silicon support, as a separate build and installer.
* Include netcdf package, for OF packages that need it.
* Reduce app size by pruning build-time-only dependencies like rust and llvm.
* Drop Python 3.9 and 3.10 support.
* Adjust app bundle name, including prerelease indicators in the name.
