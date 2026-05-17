# Systems as a Vector of Attack — TryHackMe Writeup

**Room:** Systems as a Vector of Attack
**Path:** SOC Level 1
**Completed:** May 15, 2026

Where the previous room covered humans as the entry point for attacks, this one shifts to systems themselves. It defines what
a system is in security terms, then walks through the main ways systems get compromised — vulnerabilities, supply chain
attacks, software flaws, zero-days, and misconfigurations.

## Why I Worked Through This Room

My offensive certificationshave given me hands-on exposure to exploiting systems, but this room reframes those same techniques from the defender's perspective — what types of system weaknesses a SOC analyst
needs to recognise when triaging alerts.

## What Counts as a System
a system is anything that can store digital information.

That includes the obvious — servers, workstations, laptops, mobile phones, cloud instances, databases. But it also
includes the easily overlooked — IoT devices, routers, printers, point-of-sale terminals, anything network-connected
that holds or processes data. Each of these is potential attack surface.

This framing matters because attackers don't always go for the obvious targets. Compromising a forgotten printer or a
poorly-secured IoT device often gives them a foothold to reach the systems that matter.

## Human-Led Attacks
not all attacks on systems are automated. Many are human-led, meaning an actual attacker
is hands-on-keyboard targeting a specific system or organisation.

Human-led attacks are typically:

- More targeted and adaptive than automated attacks
- Harder to detect with signature-based defences because the attacker can adjust behaviour in real time
- Often the pattern behind APT (Advanced Persistent Threat) campaigns and major breaches

For a SOC analyst, recognising the signs of a human attacker versus an automated scanner or worm is important — the
response and severity often differ significantly.

## Vulnerabilities

Vulnerabilities are weaknesses in a system that attackers can exploit to gain unauthorised access, escalate privileges,
exfiltrate data, or disrupt operations.

They come from many sources — software bugs, design flaws, missing patches, weak authentication, or simple human error
in deployment. The vulnerability itself isn't the attack; it's the doorway. The attack is what someone does with it.

## Software Vulnerabilities

A specific category: flaws in the code of an application or operating system. These can range from minor (low-impact
information disclosure) to critical (remote code execution without authentication).

Software vulnerabilities are the bread and butter of most exploitation work. They get assigned CVE identifiers, scored
by severity, patched by vendors, and tracked by SOC teams because exploitation in the wild often follows shortly after
public disclosure.

## Zero-Day Attacks

Zero-day attacks exploit vulnerabilities that are unknown to the vendor and the public — meaning no patch exists yet, and
no detection signatures have been written.

This is what makes them dangerous:

- Defenders have no signature to match against
- Patches don't exist
- They're valuable on the underground market and often reserved for high-value targets by sophisticated attackers


## Supply Chain Attacks

Supply chain attacks target a system indirectly by ncompromising a vendor, supplier, or dependency that the
target trusts.

The idea is leverage: compromise one widely-used software provider, and you get access to thousands of downstream
customers. Some of the biggest breaches of recent years have been supply chain attacks — the attacker never went near the
victim's perimeter, because the malicious code was already inside, signed and trusted.

These are particularly hard to defend against because the malicious behaviour comes from software the organisation deliberately installed and trusts.

## Misconfigurations

Not every system compromise involves a software vulnerability or a sophisticated attacker. Many breaches happen because something was simply set up wrong.

Common examples:

- Cloud storage buckets left publicly accessible
- Default usernames and passwords left enabled
- Overly permissive firewall rules
- Services exposed to the internet that should be internal
- Missing encryption on sensitive data

Misconfigurations are usually preventable, but they're extremely common — especially in cloud environments where the
pace of deployment outpaces the discipline of hardening.
Modern SOC work increasingly involves catching these issues before attackers do.

## Why This Matters for My Career Path

A few connections to SOC work:

- My offensive cert background (eJPT, eWPT, PenTest+, OSWA) is essentially a tour of how to exploit each of these
  categories — which means I understand them from the attacker's side, useful for spotting them from the
  defender's side

## Takeaways

- A system is anything storing digital information — much broader than just servers
- Human-led attacks are adaptive and harder to detect than automated ones
- Vulnerabilities, software flaws, zero-days, supply chain compromises, and misconfigurations are the main system
  attack vectors a SOC analyst will encounter
- Defending against all of them requires both signature- and behaviour-based detection

## What's Next

Continuing the SOC Level 1 path. Documenting each room here
as I work through it.

---

**Profile:** [tryhackme.com/p/Arloo](https://tryhackme.com/p/Arloo)
**Connect:** [LinkedIn](https://linkedin.com/in/charles-neboh-128496204)
