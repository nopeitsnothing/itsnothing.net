---
layout: post
title: Threat Models & OPSEC
---

...because yours is slacking.

## Good vs. Perfect

![](/images/opsec_662x436.jpg)

Operations Security (OPSEC), in one form or another, has been around for as long as there were secrets that needed to be kept. It wasn’t always called OPSEC, but the core concepts of identifying and protecting critical information have always been a deciding factor in war, in business, and countless other ventures. "Do I use an Apple device or Android?" "What versions of these are safer than the others?" "Which is the best, objectively speaking?"

Well, that's actually a very subjective way of asking that question, but the answer is that neither device or operating system (OS) is more secure than the other. That advice might seem like a non-answer to the original question, but it's integral to your OPSEC.

![](/images/opsec_700x389.jpg)

Determine your threat model AND the pretext, i.e., every detail is figured out prior to any operation because you would be the only one who knows your threat model based on certain criteria. Limiting yourself to one device, i.e, choosing to use any specific technology for communications security (COMSEC) - especially a cellphone - is bad for overall security. You would be better off using a public computer that never touches your network than you would be using a personal device, even with data wiped, cache wiped, signals blocked when not in use (airplane mode is not sufficient), etc. You could pull it off, and some OS do offer these features, sometimes hardware backed switching off of utilities can be provided as well. But you need to be able to control the interactions you have with the target. Not having access to your device as often as the interaction requires is possibly too limited an approach and you shouldn't consider ditching your communications just because your device is technically unsafe. Welcome to the world of cyber security, because you will need to utilize a plethora of data when considering your threat model.

## DREAD – For Threat Ranking

* Damage Potential: What will be the impact on exploitation?
* Reproducibility: What is the ease of recreating the attack/exploit?
* Exploitability: What minimum skill level is needed to launch?
* Affected Users: How many users will be potentially impacted?
* Discoverability: What is the ease of finding the vulnerability?

> *Note:* You may not know who your adversaries will be... or what their intentions or capabilities will be. 

Most threats are known, in fact, but that fact falls apart when you consider the potentiality of exploitation. If you have multiple proprietary devices? That's a large net in which the target could catch you, and you're relying solely on the integrity of their network and their software/hardware development and IT security (DEVOPS) to keep your information safe and secure. Each aspect of every device should separately be analyzed to determine this risk factor. Determine flaws in their network or development approach, look for errors that have unresolved issues in underlying code. 

![](/images/devops_962x590.png)

The Linux kernel, for example, doesn't suffer from source code breaches and data disclosures - it's open-source and available freely to look at by auditors. This is because the developers of the kernel support free and open source software (FOSS, as it's known). But that doesn't prevent determined threat actors from finding vulnerabilities or a bored teenager from stumbling on broken code. Then, after considering their integrity, you should look at advanced analysis of your model or network. Your threat model should be measured by following the confidentiality, integrity, and availability (CIA) triad. 

## Confidentiality

> *Note:* Only those who are authorized have access to specific assets; and that those who are unauthorized are actively prevented from obtaining access.

To explain further, consider what types of people you don't want to have access, and then feather in the ones you do. This eliminates premature threats but doesn't typically stop a determined threat actor, such as ISP or government entity, some of which have heavy resources. Who do you want to be able to access your data? Only yourself and trusted parties, on Android that isn't honored all that well, on Apple devices it is to some extent but only up to the point where they deem you a criminal - and that could mean one of several things, both benign and dangerous or destructive in nature. This should begin at setting permissions and end at setting up honeypots or access control systems, but remember, this only deters inexperienced people from trying to get your data. In the event of a breach, that's where we get the second facet of any operational structure: not only attempting to avoid the capture of information, but also to prevent the use of information should capture occur.

## Integrity

> *Note:* Ensuring that data has not been tampered with and, therefore, can be trusted. It is correct, authentic, and reliable. 

It is also secured by not just physical but digital means and is not in danger of data theft, such as using full-disk encryption (FDE) like BitLocker or Veracypt to encrypt your devices where applicable. This should start at determining the capability of your target and end at your own capability to determine when you are secure enough. Remember, it's not perfection we're striving for, only good enough. You will never have bulletproof security, even with a thousand active honeypots and a thousand man hours. And the third part:

## Availability

> *Note:* If an attacker steps past your security, what do they gain, if anything valuable or damaging to you?

Do you have contingencies? That could mean any threat, internet service provider (ISP) or DOTGOV, might access your data through unknown or undisclosed proof-of-concepts (PoCs), with almost no attack vector known to regular users of a device. Do you have multiple layers of obfuscation or encryption? Good enough, not perfect, but good enough. These things, all of which YOU must determine before ANY action is taken that is construed as criminal activity, compromise some of any mountainous number of these variables that can leave you open to threats. Simply because you favored one over the other. It's not a pie chart, it's more a chain with interwoven links - each integral to its design.

That's the CIA triad but what else should we consider before operations?

56% of the largest incidents of the last 5 years tie back to some form of web application security issue, constituting 42% of all financial losses recorded for these extreme events. 254 days is the average time-to-discovery for incidents involving web application exploits. Wow! That's a lot of time for an attacker to have control over a vector and a lot of time they could be exfiltrating data that's invaluable to your organization or to your personal security (PERSEC). Had you only placed the servers across a 30ft mote without a bridge or boat and grown wings to reach the castle but kept the wings secret from the world, you'd know this analogy is already dead in the water. In essence, there are many single points of failure involved when considering your threat model. And each is just as important as the last.

![](/images/opsec_process_768x1024.jpg)

1. *Identify* the information you need to protect
2. *Analyze* the threats
3. *Analyze* your vulnerabilities
4. *Assess* the risk
5. *Apply* countermeasures 

## Identify Security Objectives

* Confidentiality
* Integrity
* Availability
* Authentication
* Authorization
* Auditing
* Management

## Profile the Application

* Where will the application be deployed
* Who will be the Users (Actors)
* What are the Data Elements?
* What rights will the actors have?
* What Technologies will be used?
* What security mechanisms apply?

## Decompose Your Application (Generate Context)

* Trust Boundaries (indicates where trust level changes)
* Firewall (Internet -> Intranet)
* Webserver -> Database
* Your App -> External 3rd party Services
* Entry Points (Principal attack Targets)
* Ports, Pages, Components, APIs, Stored Procedures etc
* Exit Points
* Pages that display data, functions sending out values
* Data Flows
* Should we validate data at each node?

![](/images/parabola_1000x839.png)

## Identifying Threats

* Approaches to Identify Threats
* Use Attack Trees (CI4AM)
* Think like an Attacker (STRIDE/DREAD, OCTAVE etc)
* Create the threat list
* SQL Injection
* XSS
* Replay Attacks
* MITM
* Eavesdropping

## **STRIDE** – Threat Modeling

* Spoofing - Impersonating another person/process
* Tampering - Unauthorized Alterations
* Repudiation - Denying claims/unproven actions
* Information - Disclosure Exposure to unauthorized person/process
* Denial of Service - Service unavailability
* Elevation of Privileges - And/or persistence

## **DREAD** – Threat Ranking

* Damage Potential - What will be the impact on exploitation?
* Reproducibility - What is the ease of recreating the attack/exploit?
* Exploit-ability - What minimum skill level is needed to launch?
* Affected Users - How many users will be potentially impacted?
* Discoverability - What is the ease of finding the vulnerability?
