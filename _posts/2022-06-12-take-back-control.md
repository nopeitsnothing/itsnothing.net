---
layout: post
title: Take back control of your data
---

### Steps:

Embrace a zero trust model.
Don't rely on reactive security practices.
Never trust. Always verify.
Never put all your eggs into one basket.

These are ~3 things you should absolutely be doing:

**1. Better passwords:**
* go change them all, **seriously, right now!**
* use strong/non-unique passwords ([diceware](https://github.com/grempe/diceware))
* never mix or reuse them across services/accounts
* use a password manager (preferably offline, like KeePassXC)
* avoid sharing passwords and use something that notifies you of breaches
  (but don't rely solely on reactive security)
* enable 2FA/MFA, possibly use hardware keys/tokens
* backup everything just in case
* update your OS with security updates and employ active IDS/IPS (it's not as
  hard as it sounds)
* disable and/or avoid telemetry from your OS, browser and IoT devices
* don't use browser storage for sensitive info including passwords

**2. Better browsing:**
* block ads at the host level (Pi-hole, DNSSEC/DNSCRYPT, /etc/hosts, router VPN)
* uBlock Origin, LibRedirect, Smart Referrer
* ensure website integrity (in Tor, you can verify a site's /mirrors.txt)
* use a private search engine (SearXNG, DuckDuckGo, Brave)
* don't use unnecessary extensions (cf.
  [https://github.com/arkenfox/user.js/wiki/4.1-Extensions](https://github.com/arkenfox/user.js/wiki/4.1-Extensions#-dont-bother)) -
  useless bullshit
* use HTTPS (default in your regular browser usually)
* DNS over HTTPS (DOH)
* containerize and/or sanitize browsing in-between sessions, 
  (again, Arkenfox/user.js)
* minimize your footprint/fingerprint (Firefox FRP)
* plain-text emails only, question all attachments from all sources

**3. Practice your OPSEC:**
* don't login on another person's device and use privacy shields if you can
* avoid password hints or use answers that have nothing to do with them
  (confuse the enemy :))
* don't use a 4-digit pin for your devices, use a strong password
* minimize or eliminate the SMS 2FA for services to avoid SIM swaps
* avoid using your password manager for OTP
* avoid face and biometric unlocks
* never reuse usernames
* use a mail forwarding service to combat spam (and further confuse the enemy)
* [personal security checklist](https://github.com/Lissy93/personal-security-checklist)