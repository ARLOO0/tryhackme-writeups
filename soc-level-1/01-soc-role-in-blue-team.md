# SOC Role in Blue Team — TryHackMe Writeup

**Room:** SOC Role in Blue Team
**Path:** SOC Level 1
**Completed:** May 13, 2026

## TL;DR

This room covers how cybersecurity teams are organised inside
an enterprise — the reporting hierarchy from CEO down to the
analyst level, the major team structures (Red, Blue, GRC), the
specialist roles that operate around the SOC, and the
fundamental choice between running security in-house or
outsourcing to an MSSP. It's the structural map of the industry
before you go deep on any one role.

## Why I Worked Through This Room

I'm building toward a SOC analyst career and wanted to start
with the org chart before diving into frameworks and tools.
Knowing where a Tier 1 analyst actually sits in the
organisation — who they report to, who they hand off to, what
roles sit around them — makes the rest of the path make sense.

## The Security Hierarchy

The room walked through a typical enterprise security chain of
command:

- **CEO** — overall business leadership
- **CISO** (Chief Information Security Officer) — owns
  security strategy and risk for the whole organisation
- **SOC Manager** — runs the security operations function
- **Red Team Lead** — runs offensive testing
- **SOC Analyst** — front-line defensive work
- **SOC Engineer** — builds and maintains SOC tooling
- **GRC Specialist** — governance, risk, and compliance
- **Penetration Tester** — offensive testing under the Red
  Team lead

The CISO sits at the top of the security function and reports
up to executive leadership. Everything else flows from there.

## Security Departments

At a higher level, most security functions are organised into
three core departments:

- **Red Team** — offensive. Simulates real-world attacks to
  test defences.
- **Blue Team** — defensive. Detects, investigates, and
  responds to threats.
- **GRC Team** — governance, risk, and compliance. Sets
  policy, manages risk frameworks, handles audits.

These three are the pillars. Specialist roles slot into or
around them depending on the organisation's size and maturity.

## Blue Team Structure

The Blue Team itself has internal structure. The room described
a common layout:

- **SOC Manager** — leadership and oversight
- **SOC L2 Analyst** — handles escalations from L1, deeper
  investigation
- **SOC L1 Analyst** — front line, triages incoming alerts
- **SOC Engineer** — builds detection rules, maintains SIEM
  and other tooling

The flow is generally: L1 catches and triages, escalates to L2
if it's a real incident, and the SOC Engineer keeps the tooling
healthy so detection actually works.

## CIRT — Cyber Incident Response Team

When an alert turns into a confirmed incident, the CIRT (Cyber
Incident Response Team) takes over. They handle:

- Containing the incident
- Investigating root cause
- Recovering affected systems
- Reporting and lessons learned

In some organisations the CIRT is part of the SOC; in others
it's a separate dedicated team that the SOC hands incidents off
to.

## Specialist Roles Around the SOC

Beyond the core SOC structure, the room introduced several
specialist roles that operate alongside or within the broader
security function:

- **Digital Forensics Analyst** — deep investigation of
  compromised systems, evidence collection, often supports
  legal or regulatory cases
- **Threat Intelligence Analyst** — tracks adversaries, TTPs,
  IOCs; feeds intelligence into the SOC's detection capability
- **Application Security Engineer** — secures the
  organisation's software (code review, SAST/DAST,
  development pipeline)
- **AI Researcher** — increasingly common as organisations
  defend against and use AI; researches AI-based threats and
  defences

Each of these specialisations has its own career path and
typically reports up through the CISO via a relevant manager.

## Internal SOC vs MSSP

One of the more practical points in the room: not every
organisation runs its own SOC. There are two main models:

**Internal SOC**
- Built and operated in-house
- Full control over tools, processes, and people
- Direct knowledge of the business context
- Expensive to build and maintain — needs 24/7 staffing
- More viable for large enterprises with budget

**MSSP (Managed Security Service Provider)**
- External third party runs the SOC function
- Subscription-based, cheaper per-hour than full in-house
- Brings expertise and scale that smaller organisations
  can't build alone
- Less business context, more standardised processes
- Common for small and mid-size organisations, or as a
  layer on top of internal capability

Many organisations actually run a hybrid: an internal team for
business-specific work, MSSP coverage for 24/7 monitoring or
specialist services.

## What This Means for My Career Path

A few things clicked for me from this room:

- My current cert stack (BTL1, Splunk, Security+, plus the
  offensive certs) maps to **SOC L1 Analyst** as the natural
  starting role
- **SOC L2** and **CIRT** are natural progressions once I have
  experience
- The **Threat Intelligence Analyst** and **AppSec Engineer**
  roles are interesting specialisations my existing offensive
  background would support
- MSSPs are a realistic first employer in Canada later (TELUS
  Security, Bell, Arctic Wolf, eSentire), and they hire
  entry-level Tier 1 analysts in larger volume than internal
  SOCs do

Knowing the structure makes the job search clearer too — when I
read a job description now, I can place where that role sits in
the org and what the team around it likely looks like.

## Takeaways

- Security functions are organised around three pillars: Red,
  Blue, GRC — with specialists around the edges
- The Blue Team itself has clear internal tiers; the L1 role
  is the entry point most analysts start in
- CIRT handles confirmed incidents; SOC handles detection and
  triage
- Internal SOC vs MSSP is a real strategic choice for
  organisations — and from an applicant's view, MSSPs often
  offer the most accessible entry-level path

## What's Next

Cyber Defence Frameworks module next — starting with Pyramid of
Pain. Documenting each room here as I work through the SOC
Level 1 path.

---

**Profile:** [tryhackme.com/p/Arloo](https://tryhackme.com/p/Arloo)
**Connect:** [LinkedIn](https://linkedin.com/in/charles-neboh-128496204)
