# Airch v1.0 — prototype

An Arch-based desktop with an offline graphical installer, GNOME, the Airch wallpaper and Fastfetch branding, and the Necromancer, devpkgcheck and Yay toolkit.

Created and maintained by **Danny Carroll**, with AI-assisted engineering by **Codex (Elias)**. Upstream projects retain their own authorship and licenses. Danny is the final release authority.

## Download

**[Download Airch v1.0 prototype — ISO, 4.11 GiB (Google Drive)](https://drive.google.com/file/d/160A2VfMvLiVama7OEKoXFvDL6-En8heV/view?usp=sharing)**

Public viewer access and an anonymous download response were checked on October 15, 2026. Google's reported file size and whole-file CRC32C match the tested local ISO. This is an upload-integrity check, not a full downloaded SHA-256 comparison or a release signature. Google Drive displays its large-file virus-scan warning; the image is not certified malware-free.

This repository is the prototype's status/download landing page, not the complete source or build repository. The download retains its original filename, `airch-prototype-0.1-dev-x86_64.iso`. “Airch v1.0” is the public prototype label; the unchanged image still carries its internal `0.1` development/prototype identity.

The ISO is **unsigned and VM-tested**, not a stable or production release. Distribution-wide source, license and notice review is unfinished; this page does not certify redistribution readiness.

## What has passed

As of October 15, 2026, the exact image below passed:

- Offline graphical installation to a disposable 64-GiB UEFI VM disk.
- Boot from the installed disk with the ISO removed, followed by GNOME login.
- Password-required administrator access through sudo.
- Exact installed-package inventory, selected package-integrity checks, service defaults, wallpaper and plain Fastfetch checks.
- Offline launch/version checks for Necromancer, devpkgcheck and Yay.

The current Calamares package and installer configuration each passed three clean-chroot builds. Repeated successful builds are not proof of bit-for-bit reproducibility.

## Scope and known limitations

- **x86_64 UEFI; erase the selected disk only.** Installation destroys that disk's existing data. No dual boot, manual partitioning or encryption in this prototype. Start with a disposable VM.
- The live keyboard preview diagram is blank because `ckbcomp` is missing. Focused US/French/US typing tests passed.
- Online updates, real AUR transactions, physical hardware and active-install failure handling still need validation.
- Offline installation does not imply offline package updates or offline access to every AI backend or model.
- Public release signing and the remaining release reviews are not complete.

## Identify the exact prototype

Download filename: `airch-prototype-0.1-dev-x86_64.iso`  
Size: **4,417,673,216 bytes** (about 4.11 GiB)  
SHA-256:

```text
6cc3b917a43588bf3482137406b85b2cf399b101f5dcea30806ee24f17e36278
```

Compare the downloaded file:

```sh
sha256sum 'airch-prototype-0.1-dev-x86_64.iso'
```

The result must match the hash above. A checksum detects differing bytes; it is not a release signature.
