# Octave.app CHANGELOG

This is the changelog for Octave.app, the native Mac app bundle of GNU Octave.

This has info about the user-facing changes in the app itself. It doesn't include developer info about the build tools used to create Octave.app; see the octave-app-bundler repo for that.

## 9.1.0

* Add a bare `octave` link to the internal `usr/bin` directory.
* Remove versioned llvm package that was accidentally included and inflating the app size.
* Built on macOS 12.
  * For better compatibility across OS versions.
  * Fixes "missing perl5.34" breakage in the test suite on macOS 12.
* Drop librsvg package, to reduce app size.

## 8.4.0 (2024-05-02)

* First 8.x (or even 7.x) release.
* Drop gnuplot graphics back-end.
* Add native Apple Silicon support, as a separate build and installer.
* Include netcdf package, for OF packages that need it.
* Reduce app size by pruning build-time-only dependencies like rust and llvm.
* Drop Python 3.9 and 3.10 support.
* Adjust app bundle name, including prerelease indicators in the name.
* Move `octave_app_diagnostic_dump` tool to package-qualified `octapp.diagnostic_dump`.
