# NEXT System Control — Public Releases

Official public downloads for NEXT System Control PS4 homebrew. This repository contains release information and package downloads only; the development source and Git history remain private.

## Latest release — v0.5.0 Beta 2

**[Download NEXT System Control Beta 2 PKG](https://github.com/killernos/NEXT-System-Control-Releases/releases/download/v0.5.0-beta.2/NEXT.System.Control.v0.5.0.Beta.2.pkg)**

[Beta 2 release notes](https://github.com/killernos/NEXT-System-Control-Releases/releases/tag/v0.5.0-beta.2) · [All releases](https://github.com/killernos/NEXT-System-Control-Releases/releases) · [Official website](https://killernos.github.io/NEXT-System-Control-Website/)

**Package:** `NEXT.System.Control.v0.5.0.Beta.2.pkg`  
**SHA-256:** `0d6cca91b8f2c4958915fcc9805aaac606534d8db4e7a0f8752d0490333fd3f3`  
**PS4 title ID:** `NEXT00034` (side-by-side test package; verify it is unused before installation)

### What's new in Beta 2

- Controller-driven dashboard theme selector and Tool Library
- Six selectable themes with saved preferences
- Explorer/Developer startup selector refinements
- Dashboard icon alignment improvements

### Validation

The PC simulator regression suite passed 6/6 tests, and the OpenOrbis ELF/FSELF build and package generation completed. A PS4 user reported that this Beta 2 build works, but firmware, test count, and individual hardware coverage were not recorded. **Broader firmware compatibility is not verified.**

## Previous release — v0.5.0 Beta 1

- [Beta 1 release notes](https://github.com/killernos/NEXT-System-Control-Releases/releases/tag/v0.5.0-beta.1)
- [Download Beta 1 PKG](https://github.com/killernos/NEXT-System-Control-Releases/releases/download/v0.5.0-beta.1/NEXT.System.Control.v0.5.0.Beta.1.pkg)
- SHA-256: `af0c27c878172acbc1d82d220b440764cf65f2c4b77cedad9035780d6c571b09`

Beta 1's Revision 21 testing was reported on firmware 12.00 with GoldHEN and separately on 13.52 (GoldHEN configuration not specified for 13.52).

## Installation and safety

1. Review the release notes and confirm your console's firmware and setup are appropriate.
2. Verify the downloaded PKG checksum and the title ID before installing.
3. Back up important data and install using your usual trusted PS4 package installation workflow.
4. Enable network services only when needed, on a trusted isolated local network.

**Beta limitations:** This is not a stable production release. FTP is unencrypted; do not expose SSH or FTP to the internet. Filesystem access remains limited. This release does not enable unrestricted filesystem modifications or automatic privilege elevation. Compatibility varies by console.

## Repository scope

This is a **public releases-only** repository. The private `killernos/NEXT-System-Control` development repository, its source, and its Git history are not distributed here. GitHub automatically offers source archives of this small public releases repository alongside release assets.
