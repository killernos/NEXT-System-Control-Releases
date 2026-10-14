# NEXT System Control — Public Releases

This repository distributes signed NEXT System Control release packages and
release information only. It does not contain the private development
repository, its source code, or its Git history.

## Latest release

**v0.5.0-beta.2** is a beta package for PlayStation 4. Beta 2 adds the controller-driven dashboard theme selector and Tool Library, six selectable themes with saved preferences, and refinements to the Explorer/Developer startup selector and dashboard icon alignment.

The user reports that this Beta 2 build works on PS4. Firmware, test-cycle count, and individual test coverage were not recorded; compatibility outside that limited report is unverified.

- [Release notes and package](https://github.com/killernos/NEXT-System-Control-Releases/releases/tag/v0.5.0-beta.2)
- [Download the PKG](https://github.com/killernos/NEXT-System-Control-Releases/releases/download/v0.5.0-beta.2/NEXT.System.Control.v0.5.0.Beta.2.pkg)
- SHA-256: `0d6cca91b8f2c4958915fcc9805aaac606534d8db4e7a0f8752d0490333fd3f3`

## Installation

1. Review the release notes and confirm this beta is appropriate for your console setup. The recorded hardware validation is limited to the user's report that this build works; firmware and test details were not recorded.
2. Download `NEXT.System.Control.v0.5.0.Beta.2.pkg` and transfer it to the console using your normal, trusted local installation workflow.
3. Confirm the package title ID `NEXT00034` is unused on your console, then install it with the console's package installer and launch NEXT System Control.
4. Enable network services only when needed. Keep them on a trusted local network; never forward their ports to the internet.

Back up important data before installing beta software. Installation and compatibility behavior may vary by console setup.

## Beta limitations and safety

- This is beta software, not a stable production release.
- Hardware validation is limited to the user report noted above; no firmware compatibility claim is made.
- FTP traffic is not protected by TLS. Use it only on a trusted, isolated local network and only when needed.
- SSH and FTP must not be exposed to the public internet.
- Filesystem access remains limited; the filesystem browser does not enable unrestricted filesystem modification.
- Privileged operations require explicit authorization; this release does not automatically elevate privileges.

## Repository scope

This is a release-distribution repository. Development source and its history
remain in the private
[NEXT-System-Control](https://github.com/killernos/NEXT-System-Control)
repository and are not copied here.
