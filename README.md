# NEXT System Control — Public Releases

Official public downloads for NEXT System Control PS4 homebrew. This repository contains release information and package downloads only; the development source and Git history remain private.

## Latest release — v0.5.0 Beta 3 (Debugger Diagnostic)

**[Download NEXT System Control Beta 3 PKG](https://github.com/killernos/NEXT-System-Control-Releases/releases/download/v0.5.0-beta.3/NEXT.System.Control.v0.5.0.Beta.3.pkg)**

[Beta 3 diagnostic notes](https://github.com/killernos/NEXT-System-Control-Releases/releases/tag/v0.5.0-beta.3) · [All releases](https://github.com/killernos/NEXT-System-Control-Releases/releases) · [Official website](https://killernos.github.io/NEXT-System-Control-Website/)

**Package:** `NEXT.System.Control.v0.5.0.Beta.3.pkg`

**SHA-256:** `39321070369745287b3ce0f93102444b1df43a7ef4c2927db69fee101c6260d5`

**PS4 title ID:** `NEXT00053` (a separate application entry from earlier builds).

**Important diagnostic result:** the maintainer tested this exact package on
PS4. NEXT targeted the detected console-local IPv4 on TCP 744, but the
connection was refused (`errno 61`). This does not confirm that ps4debug-NG
started or that a server is listening; Beta 3 is published as a diagnostic
build, not as a claim that debugger connectivity is fixed.

### Beta 3 diagnostic change

- Manual read-only debugger queries use the console's freshly detected local
  IPv4 address on TCP port 744 instead of assuming PS4 loopback routing.
- The address comes from NEXT's network snapshot; arbitrary remote targets are
  not accepted.
- No query runs automatically; the user must request it from the diagnostic
  screen. NEXT does not load or resend a payload, attach to processes, access
  process memory, alter the kernel, or elevate privileges.

OpenOrbis PS4 compilation, FSELF, package generation, ASan/UBSan debugger
tests, the real Linux loopback protocol test, and UI regression test passed.

- [Release notes and package](https://github.com/killernos/NEXT-System-Control-Releases/releases/tag/v0.5.0-beta.3)
- [Download the PKG](https://github.com/killernos/NEXT-System-Control-Releases/releases/download/v0.5.0-beta.3/NEXT.System.Control.v0.5.0.Beta.3.pkg)
- [Diagnostic details](v0.5.0-beta.3.md)

## Previous release — v0.5.0 Beta 2

- [Beta 2 release notes](https://github.com/killernos/NEXT-System-Control-Releases/releases/tag/v0.5.0-beta.2)
- [Download Beta 2 PKG](https://github.com/killernos/NEXT-System-Control-Releases/releases/download/v0.5.0-beta.2/NEXT.System.Control.v0.5.0.Beta.2.pkg)
- SHA-256: `0d6cca91b8f2c4958915fcc9805aaac606534d8db4e7a0f8752d0490333fd3f3`

## Earlier release — v0.5.0 Beta 1

- [Beta 1 release notes](https://github.com/killernos/NEXT-System-Control-Releases/releases/tag/v0.5.0-beta.1)
- [Download Beta 1 PKG](https://github.com/killernos/NEXT-System-Control-Releases/releases/download/v0.5.0-beta.1/NEXT.System.Control.v0.5.0.Beta.1.pkg)
- SHA-256: `af0c27c878172acbc1d82d220b440764cf65f2c4b77cedad9035780d6c571b09`

Beta 1's Revision 21 testing was reported on firmware 12.00 with GoldHEN and separately on 13.52 (GoldHEN configuration not specified for 13.52).

## Installation

1. Download the desired PKG from the relevant release's assets. Beta 3 is a
   diagnostic build; review its known result before installing.
2. Transfer it to your jailbroken PS4 using your usual installation workflow
   and install it with the PS4 package installer.
3. Launch NEXT System Control.

Beta 3 package title ID: `NEXT00053`, a separate application entry from earlier
builds. Beta 2 remains available with title ID `NEXT00034`.

## Network use

Enable SSH or FTP only when needed on a trusted local network. FTP is not
TLS-encrypted; do not expose either service to the public internet.

## Release publication checklist

Every authorized release includes the public package, detailed release notes,
and an updated [project website](https://killernos.github.io/NEXT-System-Control-Website/).

1. Confirm the maintainer has tested the exact package on PS4 before release.
2. Describe the actual additions, changes, and fixes, with useful controls and
   concise installation steps. Use a clear testing statement; do not speculate
   about unreported firmware support or add generic beta disclaimers.
3. Publish the package and notes here, preserving earlier releases. Verify the
   public download's filename, size, and SHA-256.
4. Update this README, the versioned release-notes document, and the website's
   latest-release headings, highlights, and download links together.
5. Merge the public documentation and website updates with approval, wait for
   GitHub Pages deployment, and verify the live site and release page agree.
   A release announcement is not complete while the live website is outdated.
6. Keep private application source and history out of these public repositories.

## Repository scope

This is a **public releases-only** repository. The private `killernos/NEXT-System-Control` development repository, its source, and its Git history are not distributed here. GitHub automatically offers source archives of this small public releases repository alongside release assets.
