# NEXT System Control — Public Releases

This repository distributes signed NEXT System Control release packages and
release information only. It does not contain the private development
repository, its source code, or its Git history.

## Latest release

**v0.5.0-beta.1** is a beta package for jailbroken PlayStation 4 consoles.
Hardware testing has been confirmed on firmware **12.00 with GoldHEN** and
also on firmware **13.52**. The GoldHEN configuration for the 13.52 test was
not specified. Other firmware versions and hardware configurations are
unverified.

- [Release notes and package](https://github.com/killernos/NEXT-System-Control-Releases/releases/tag/v0.5.0-beta.1)
- [Download the PKG](https://github.com/killernos/NEXT-System-Control-Releases/releases/download/v0.5.0-beta.1/NEXT-Stage7-Revision21.pkg)
- SHA-256: `af0c27c878172acbc1d82d220b440764cf65f2c4b77cedad9035780d6c571b09`

## Installation

1. Confirm the console is a jailbroken PS4 running firmware 12.00 or 13.52.
   GoldHEN was confirmed for the 12.00 hardware test; configuration details
   for the 13.52 test were not specified. Other firmware versions and
   configurations are unverified for this beta.
2. Download `NEXT-Stage7-Revision21.pkg` and transfer it to the console using your normal,
   trusted local installation workflow.
3. Install it with the console's package installer and launch NEXT System
   Control.
4. Enable network services only when needed. Keep them on a trusted local
   network; never forward their ports to the internet.

Back up important data before installing beta software. Installation and
compatibility behavior may vary by console setup.

## Beta limitations and safety

- This is beta software, not a stable production release.
- Hardware testing has been confirmed on firmware 12.00 with GoldHEN and
  separately on firmware 13.52. The 13.52 GoldHEN configuration was not
  specified. No compatibility claim is made for other firmware versions.
- FTP traffic is not protected by TLS. Use it only on a trusted, isolated
  local network and only when needed.
- SSH and FTP must not be exposed to the public internet.
- The filesystem browser supports a limited set of directories.
- The filesystem browser does not enable root privilege transitions or
  unrestricted filesystem modification.
- Normal application exit behavior still needs compatibility testing across
  configurations.

## Repository scope

This is a release-distribution repository. Development source and its history
remain in the private
[NEXT-System-Control](https://github.com/killernos/NEXT-System-Control)
repository and are not copied here.
