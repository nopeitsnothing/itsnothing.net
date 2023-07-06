---
layout: post
title: What's a SIM card, and how do I secure it?
---

## Perceived SIM card OPSEC

SIM cards provide a degree of privacy by allowing users to control their identity and access to mobile services, but users should also be mindful of other potential privacy risks and take appropriate measures to protect their personal information.

The Subscriber Identity Module is a topic which I have talked about on my blog before, but never at length. I've talked about what to do to prevent, or significantly lower the risk of, SIM swaps. But what are SIM cards? What do they store, really? I usually don't find the need to talk about SIM cards in the realm of cybersecurity. However, it poses an interesting topic as it has received a rise in popularity as a threat rather than a convenience. Here, I will discuss the increase in cyberattacks targeting mobile phones, specifically SIM cards: (1) how do they work and (2) how do attackers leverage them for profit?

This post is not to inform hackers on techniques, tools, and procedures (“TTPs”), but rather it should be considered an informative article on the dangers of mobile phones realistically, not just as some tinfoil persona. The cellular devices that you know and use (and likely carry everywhere) are not impervious to spyware, malware and unwanted behavior, however, most people don't fully understand these risks and the importance of having the knowledge of how to protect your phones. Some dangers involved in carrying a mobile device include tracking, spyware, surveillance, and even stalking. We'll discuss these all in depth, and we'll also discuss ways to prevent them, or at least decrease the likelihood of being targeted by individuals, corporations, and even the government.

## Origins of the SIM card and necessity on cell networks

In the early 1990s, GSM (Group systems for mobile communications) was developed as a standard for mobile communication. It introduced the 2G protocol, which became widely used in smartphones. The first deployment of GSM took place in Finland in December 1991. Over time, GSM [evolved into 3G and 4G technologies](https://www.wired.com/2010/06/wired-explains-4g/). SIM (Subscriber Identity Module) cards are used to store user information such as IMSI, ICCID, Authentication Key, Location Area Identity (LAI), and national emergency call operator details. SIM cards provide identification and authentication across different telecom operators and incorporate [COMP128v1](https://en.wikipedia.org/wiki/COMP128) authentication algorithms, including A3 for network security and A8 for encryption keys related to authentication key security. SIM cards come in different versions, including standard, micro, and nano.

1. Standard SIM: The standard SIM card, also known as a mini SIM, is the traditional form factor used in older mobile devices. It is larger in size compared to the newer versions and is gradually being phased out in favor of smaller SIM card types.
2. Micro SIM: The Micro SIM card is smaller than the standard SIM and was introduced to accommodate slimmer smartphones. It retains the same functionality as the standard SIM but has a reduced form factor.
3. Nano SIM: The Nano SIM card is the smallest SIM card type currently available and is commonly used in modern smartphones. It is significantly smaller than both the standard and micro SIM cards and requires specialized tools to handle due to its compact size.

SIM cards play a crucial role in the interaction between mobile devices and the GSM network. When a SIM card is inserted into a mobile device, it provides the necessary identification and authentication information for the device to connect to the GSM network. The SIM card stores essential data such as the International Mobile Subscriber Identity (IMSI), Integrated Circuit Card ID (ICCID), and authentication key. This information allows the device to establish a secure connection with the network and access services like voice calls, messaging, and mobile data. The GSM network uses the SIM card's information to verify the user's identity, authorize network access, and apply specific service features based on the user's subscription. This interaction ensures the seamless functioning of mobile devices within the GSM network, enabling communication and access to various network services.


## Real risks of SIM cards and its implications

By using the SIM card, customers can have a level of control over their personal information and access to mobile services. The SIM card allows customers to switch between different mobile devices while retaining their identity and subscribed services. This offers a level of privacy and convenience.

However, it's important to note that while SIM cards provide some privacy protection, they do not guarantee complete privacy. Mobile network operators and authorized parties can still access certain information stored on the SIM card, such as call records and location data, for legitimate purposes like billing and providing network services. Additionally, SIM cards are subject to security vulnerabilities and can be targeted by hacking or unauthorized access attempts.

Why are hackers targeting SIM cards? Mostly for fraud, and otherwise profit. The SIM contains its own microprocessor (CPU), program memory (ROM), working memory (RAM), data memory (EPROM or E2PROM), and serial communication module. The SIM card interacts with the mobile device through a serial Input/output (I/O) connection, serving as a communication link. The T0 protocol is commonly used, defining the electrical coding for commands and responses between the mobile device and SIM card. The SIM card operates in a passive role, responding to commands from the mobile device and providing “Status Words” as responses. It cannot initiate communication with the device independently.

SIM cards pose several [threats to personal information security](/2022/01/27/A-proper-threat-model.html):

1. **Confidential information**: SIM cards can store sensitive data like login IDs, passwords, and messages related to bank accounts and social networking sites, making them potential targets for unauthorized access and identity theft.
2. **Personal and professional data**: SIM cards may contain personal and professional messages, important contact information, and call logs. If accessed by unauthorized individuals, this information could be exploited for malicious purposes.
3. **Deleted data recovery**: deleted messages can potentially be recovered from SIM cards, posing a risk of privacy breaches even after data deletion.
4. **Data persistence**: SIM card data is resistant to various environmental conditions such as heat, flame, dust, moisture, stains, and magnetic fields. This persistence makes it difficult to destroy the data stored on a SIM card through ordinary means.
5. **Physical damage**: while scratches and striations may not render a SIM card unreadable, physical damage inflicted by compression marks, such as from a stone or hammer, can make the card unreadable. I prefer to use a screwdriver or drill if I have time to spare. Screwdriver and hammer to split the "fibers" of embedded chips and capacitors, and a drill to completely penetrate and destroy the platters of storage devices.
6. **Data recovery**: even if a SIM card becomes unreadable or damaged, it can potentially be read by replacing the EEPROM chip into a new SIM card or by using proper probing techniques. This highlights the need for proper disposal or secure handling of old SIM cards.

To protect private data from being easily stolen using a SIM card reader, *it is recommended to break the SIM card into two pieces* before discarding it, making it significantly harder for strangers or criminals to access private information.

To prevent forensic recovery and ensure the secure disposal of a SIM card, *it is recommended to follow a thorough process that involves physical destruction*. Here is an in-depth description of the process:

## Protecting yourself against forensics

You will need a pair of pliers, scissors, or a sharp knife, as well as safety gloves to protect your hands. Remove the SIM card from the mobile device. Power off the mobile device and locate the SIM card slot. You will use a SIM card ejector tool or a small paperclip to remove the SIM card from the device.

First, disable the SIM card: access the device settings. Disable any security features or PIN codes associated with the SIM card. This step ensures that the SIM card does not prompt for authentication when attempting to access the data. When you've removed the SIM, physically destroy it by placing it on a flat and sturdy surface, and, using the pliers, scissors, or a sharp knife, applying pressure or cut through the SIM card. Start by severing the gold contacts and then proceed to cut or break the rest of the card into multiple pieces. Make sure to apply enough force to render the card irreparable. Dispose of the SIM card safely: once the SIM card is completely destroyed, separate the broken pieces. It is advisable to dispose of the pieces in separate trash bins or through different waste collection methods. This helps further ensure that the card cannot be reconstructed or retrieved. Remember, failure to dispose of SIM cards can result in retrieval of sensitive data. It is very important to not only physically destroy it but also *not to leave the pieces in the same bin*. If it's not incinerated or degaussed, you should always use at least two bins.

By following this process, you significantly reduce the chances of forensic recovery and unauthorized access to the data stored on the SIM card. However, it's critical to note that physical destruction does not guarantee absolute security, and if highly sensitive data is involved, additional precautions may be necessary, such as incineration or professional destruction services.

## To protect yourself, follow these practices

**Use strong authentication**: set a strong alphanumeric passcode for your SIM card to prevent unauthorized access, or at the very least, use a long PIN. This adds an extra layer of security, ensuring that even if your device is lost or stolen, your SIM card remains protected. Most telecoms will allow a registration PIN or subscriber PIN to prevent unauthorized changing of your number or inserting into a new device without your permission. This is one of the most important steps in this article.

**Enable two-factor authentication (2FA)**: whenever possible, enable 2FA for your mobile services. This is an additional step for authentication, typically involving a verification code sent to your SIM card, further securing your identity and preventing unauthorized access. You can use [TOTP](https://en.wikipedia.org/wiki/Time-based_one-time_password) (time-based authentication mechanism) or something like a [hardware key](https://www.yubico.com/) from Yubico. Store your TOTP separate from your passwords and do not keep them in your password manager, as any unauthorized access to your manager would lead to compromise of the sensitive time-based codes as well.

**Regularly update software and firmware**: keep your mobile device's software and firmware up to date. Updates often include security patches and bug fixes that help protect against potential vulnerabilities and threats.

**Be wary of phishing attempts**: exercise caution when receiving text messages, emails, or phone calls asking for personal or sensitive information. Telecom providers typically do not request such information through unsolicited communications. Be vigilant and avoid sharing personal information unless you can verify the legitimacy of the request. Your bank and your telecom provider will never ask for your sensitive details over the phone. If they do, consider that it isn't in your best interest to share anywhere but in person to a credentialed employee or technician.

**Monitor account activities**: regularly review your mobile service account activities, such as call logs, text message records, and data usage. If you notice any suspicious or unfamiliar activities, report them to your telecom provider immediately. You have the option to subscribe to services that can do this for you, either manually or automatically, like [Delete Me](https://joindeleteme.com/).

**Secure network connections**: when accessing the internet or using mobile data, connect to secure and trusted networks. Avoid using public Wi-Fi networks, which can be susceptible to eavesdropping and data interception. Consider using a virtual private network (VPN) for additional privacy and encryption. **VPNs do not offer anonymity.** You could also consider use of [SafingIO's SPN](https://safing.io/) Anonymity can only be offered by proper onion routing via [the Tor network](https://www.torproject.org/) or [the i2p network](https://geti2p.net/en/).

**Protect Physical Security**: keep your mobile device and SIM card in a secure location, such as a safe or loclbox. Avoid lending your device to others or leaving it unattended in public places. Do not hand your devices to strangers to make calls becasue this is a tactic used by thieves. You'd think this is common sense, but it has been used before to nab physical devices from darknet vendors and admins. Physical security of your device helps prevent unauthorized access. By following these measures, you can enhance the protection of your identity at the telecom level while using a SIM card, reducing the risk of identity theft, unauthorized access, and fraudulent activities.

In conclusion, protecting your identity while using a SIM card requires a combination of proactive measures and responsible practices. By implementing strong authentication, enabling two-factor authentication, keeping your software up to date, being vigilant against phishing attempts, monitoring account activities, securing network connections, and maintaining physical security, you can significantly enhance the protection of your personal information. Besides the registration PIN at your provider, which can be a real life-saver, remember to dispose of old SIM cards properly by physically destroying them to prevent forensic recovery. By taking these precautions, you can enjoy a safer and more secure mobile experience, reducing the risk of identity theft and unauthorized access to your sensitive data.

## References

1. Huurdeman, A. A. (2003). _The Worldwide History of Telecommunications_. John Wiley & Sons.

2. Gudimalla, T. K. M., P, V., & Kannan, S. (2019). Survey Analysis of Cloned SIM Card. _SSRN Electronic Journal_. [https://doi.org/10.2139/ssrn.3431642](https://doi.org/10.2139/ssrn.3431642)

3. Oyediran, O., Omoshule, A., Misra, S., Maskeliūnas, R., & Damaševičius, R. (2019). Attitude of mobile telecommunication subscribers towards sim card registration in Lagos State, Southwestern Nigeria. _International Journal of System Assurance Engineering and Management_, _10_(4), 783–791. [https://doi.org/10.1007/s13198-019-00809-6](https://doi.org/10.1007/s13198-019-00809-6)

4. Srivastava, A., & Vatsal, P. (2016). Forensic Importance of SIM Cards as a Digital Evidence. _Journal of Forensic Research_, _07_(02). [https://doi.org/10.4172/2157-7145.1000322](https://doi.org/10.4172/2157-7145.1000322)
