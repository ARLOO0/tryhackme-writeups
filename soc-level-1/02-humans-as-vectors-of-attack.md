# Humans as Vectors of Attack — TryHackMe Writeup

**Room:** Humans as Vectors of Attack
**Path:** SOC Level 1
**Completed:** May 13, 2026

## TL;DR

This room covers the most consistently exploited part of any security stack: people. It walks through why humans are the
weakest link, how attackers target them through social engineering, and the defensive thinking required to protect
against attacks that bypass technology by going straight at the user.

## Why I Worked Through This Room

Continuing the SOC Level 1 path. I've spent a lot of time studying technical attack techniques through my offensive
certifications, but a large share of real-world incidents start with someone clicking a link or trusting the wrong
voice on a phone call. Understanding the human attack surface is foundational SOC analyst knowledge.

## The Human Element

Humans are the weakest link in cybersecurity. No matter how mature an organisation's technical controls are — firewalls,
EDR, SIEM, MFA — a single person clicking the wrong attachment or trusting the wrong caller can bypass all of it.

## Social Engineering

Attacks that target humans rather than technology are collectively called social engineering. Instead of finding a
software vulnerability, the attacker finds a behavioural vulnerability — exploiting trust, fear, authority, or
curiosity.


## Phishing Attacks

Phishing is one of the most common social engineering techniques. Attackers send messages that appear legitimate
to trick recipients into:

- Clicking malicious links
- Opening malicious attachments
- Entering credentials on fake login pages
- Authorising actions they wouldn't normally take

Phishing remains effective because well-crafted emails can look almost identical to legitimate communications from
banks, employers, IT teams, or service providers.

## Malware Downloads

A successful phishing attack often leads to malware delivery. The user clicks a link or opens an attachment, and the system
gets infected — leading to outcomes like:

- Credential theft
- Lateral movement across the network
- Data exfiltration
- Ransomware encryption


## Deepfakes

Deepfakes are an evolving threat — AI-generated audio, video, or images used to impersonate real people convincingly.

What makes them particularly dangerous is that they exploit the deepest layer of human trust: what we see and hear. A voice that sounds like a CEO authorising a wire transfer, or
a video call that appears to be a senior executive, can bypass even cautious users.

Organisations have lost millions to attacks where the attacker convincingly impersonated leadership through deepfake voice or video.

## Defending Humans: Detection and Mitigation

Defence against human-targeted attacks has two parts:

**Detection** — identifying when an attack is in progress or has succeeded. SOC teams play a central role here, watching
for the signals that a user has clicked something, downloaded something, or entered credentials somewhere they shouldn't.

**Mitigation** — reducing the damage when an attack does succeed, and reducing the likelihood of success in the first
place. This includes user training, technical controls like email filtering and MFA, and incident response procedures
that contain damage fast.

Neither layer is enough on its own. Detection without mitigation means you see the attack but can't stop it.
Mitigation without detection means you've reduced risk but won't know when something slips through.

## Why This Matters for My Career Path

A few takeaways that connect directly to SOC work:
- Understanding social engineering helps me read alerts in context: an unusual login from a new country becomes more
  suspicious when paired with a phishing email reported by the same user
- Deepfakes are a current and growing concern — staying current on this is part of staying employable in SOC work
  over the next 3-5 years

## Takeaways

- Humans are the weakest link by default, but they're also the most leverage-able defensive layer if trained well
- Social engineering is the umbrella; phishing, malware delivery, and deepfakes are specific techniques under it
- SOC defence against human-vector attacks requires both detection and mitigation working together
