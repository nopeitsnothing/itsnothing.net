---
layout: post
title: Protect Yourself From SIM Swaps
---

"...why can't I make calls? I just paid my bill."

It can be a legitimate thing provided by a cell service provider on request of a customer. When a device is stolen, they can perform a swap using a new card in a separate device. This is useful because you can have your old details sent to the new device when you login to your given Google or Apple account.

The problem is that hackers have found a way to exploit this practice by calling in to your service provider (e.g., Boost Mobile/[Sprint CARE](https://www.sprint.com/en/support/contact-us.html) customer line). All they need to do is say your device was stolen and give your details. The carrier then deactivates your [legitimate] device. They reinstate service for your account on the hacker's device or emulator. They can now pretend to be you when receiving OTP codes from your accounts to bypass 2FA requirements. 

![](/images/phone_850x538.jpg)

You will know if you're a victim because you will lose all internet connectivity to the device. You will lose the ability to make calls, receive texts and send calls, etc. You need to be smart and quick to protect both your data and your identity. 

## Immediately call your bank

Your funds are [in immediate danger](https://www.paypal-community.com/t5/Disputes-and-Limitations/Hacked-mobile-phone-account-fraud-on-Paypal/td-p/2717306) and are the [obvious first thing](https://www.forbes.com/sites/quora/2019/06/04/how-are-criminals-using-smart-devices-to-commit-crimes/) to which a smart criminal would want to gain access. Tell them you're requesting a credit and checking freeze. This should prevent the attacker using your accounts for purchases and other fraudulent purposes. ID theft sucks and it's hard to stop once it's started and it will wreak hell on your life. Also, you might wish to place holds on your current cards, as difficult at it will be too mane legitimate purchases for the next days or weeks, it's nothing compared to losing your entire savings and other accounts to overdraft fees, etc. 

## Move accounts to a separate email

Attempt to [forward all incoming mail](https://alternativeto.net/feature/alias-support/) from your other email to the new one and cease saving copies of all mail. Immediately switch to using your devices to save email. This prevents an attacker from reading new emails and resets. 

## You can now reset all passwords safely

...without risking an attacker simply intercepting reset requests and negating your efforts to regain control. Change passwords to all accounts and [disable 2FA via SMS](https://krebsonsecurity.com/2021/03/can-we-stop-pretending-sms-is-secure-now/) and [email](https://superuser.com/questions/1712246/how-can-i-intercept-not-just-monitor-http-requests-responses-so-that-i-can-edi). Switch to the preferred method of using OTP for authentications. You can use Yubikey, Google authenticator or Authy, to name a few. Also immediately disconnect your phone from all accounts and leave it disconnected at least for now. Change all passwords before proceeding and use strong passwords. You really should use a password manager. I personally use Dashlane but you can use your preferred app or service. For those services you, for some reason, you can't change the passwords, call their CSR line. Do NOT use LastPass. They have suffered a probable breach and users are reporting theft of master passwords. 

## Now file a police report

![](/images/police_1600x1236.jpg)

This is a crime. You are a victim and you need to report the activity of the attacker. In most cases, they will investigate the caller to the service provider and trace the number. This may or may not help lead to an arrest and it will give you some peace of mind, but it's one of the most important steps aside from the next one. The police will give you further instructions and keep you in the loop during any investigations. In the future, be advised that you can get protection from ID theft with some homeowners insurance policies. Just something to consider.

![](/images/2FA_shield_706x394.jpg)

## Don't use SMS for 2FA - ever

It isn't considered secure, it's only considered fast and easy. Stop being the guy that uses SMS-based authentications for all accounts, especially Google or Apple accounts. By all means, any effective takeover of those “main” accounts would be a nightmare to fix, so be proactive instead of [reactive](https://haveibeenpwned.com/). Setup an external key system for your Google and Apple accounts. Hardware and software solutions are available for authentication devices. 

## Consider your options

You can also get a Google Voice or other [VoIP](https://telnyx.com/resources/how-to-get-a-voip-number) number to use only for 2FA. These are not tied to your direct identity and can't be SIM swapped by attackers. This is one way to prevent it altogether but [not everyone likes relying on Google](https://www.privacyguides.org/en/email/), however secure they are, because they're also data mining [every bit you transfer](https://www.theverge.com/2013/7/17/4517480/nsa-spying-prism-surveillance-cheat-sheet). Alternative ways for prevention could include using a burner phone you only utilize for 2FA. It contains a different SIM and is not likely to be attacked easily (prepaid is best here). This is up to you. I use a hardware key device for my Google and I use a software OTP from Authy for others that aren't as important.

Read: still important enough to protect, just not as evil as losing my main Google account. Consider your threat model when deciding this. Authentication apps that store seeds on your device and not on a centralized server network are preferred. They're on your device only. 

[Multi-factor authentication keys](https://www.privacyguides.org/en/multi-factor-authentication/) are becoming huge with the advent of U2F (universal two-factor). It consists of a physical device, a USB key, which is stored on your person or in a secure environment such as a safe or lockbox. You need to insert it into your laptop or desktop computer to log in to accounts. No typing necessary. In the future these will support NFC and Bluetooth. 

## Recovery keys and codes

Your *last resort* should be a recovery phrase or codes. Some apps already enable these by default but they may or may not provide safety for your accounts. They're not viable if you don't know where they are 100% of the time and they're not secure on your physical devices and your person. Again, consider your threat model. What's useful for a forgetful child isn't useful for a journalist that might be compelled in a foreign country to give the codes to their interrogator.
