---
layout: post
title: What exactly does Windows collect on you? Well..
---

**Just from one angle, the Bluetooth and Wi-Fi?**

Geo-location via Wi-Fi & Bluetooth: Whether it is Android, iOS, Windows,
macOS, or even Ubuntu. Most popular Operating Systems now collect telemetry
information by default even if you never opt-in or opted-out from the start.
Some like Windows will not even allow disabling telemetry completely without
some technical tweaks. This information collection can be extensive and
include a staggering number of details (metadata and data) on your devices
and their usage.

**Itemized lists**:
- [Full list of required diagnostic data](https://docs.microsoft.com/en-us/windows/privacy/required-windows-diagnostic-data-events-and-fields-2004)
- [Full list of optional diagnostic data](https://docs.microsoft.com/en-us/windows/privacy/windows-diagnostic-data)

**Mitigation:**

**W10Privacy:**
- Download and install [W10Privacy](https://www.w10privacy.de/english-home/)
- **Right-click** > **Run as administrator**
- Check all the recommended (Green) settings and save.
- Optional but recommended (but could break things, use at your own risk), also
check the orange/red settings, and save.
- **Reboot**

**WindowsSpyBlocker:**
- Download and run [WindowsSpyBlocker](https://crazymax.dev/WindowsSpyBlocker/download/)
- Type **1** and go into **Telemetry**
- Type **1** and go into **Firewall**
- Type **2** and add **Spy Rules**
- **Reboot**

**Also, consider using O&O ShutUp10++:**
- Download and run [O&O ShutUp10++](https://www.oo-software.com/en/shutup10)
- Enable _at least_ all of the recommended settings.

**Settings** > **Privacy** > **Diagnostic** > **Delete all Data**

**You will need to update and re-run W10Privacy and WindowsSpyBlocker frequently
 and after any Windows update as they tend to silently re-enable telemetry using
 those updates.**

As a bonus, it could be interesting to also consider
[hardening your Windows host](https://github.com/beerisgood/windows10_hardening).
(This is a security guide, not a privacy guide.)

**[The Hitchhiker's Guide to Online Anonymity](https://anonymousplanet-ng.org/)**

Disclaimer: I am a maintainer.
