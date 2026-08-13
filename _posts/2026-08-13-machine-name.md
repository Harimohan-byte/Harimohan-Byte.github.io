---
title: "Machine Name — HackTheBox / TryHackMe Writeup"
date: 2026-08-13 12:00:00 +0530
categories: [HackTheBox, Linux]
tags: [web, privilege-escalation, ssh, cve]     # lowercase, hyphenated tags
---

> Only publish this writeup after the machine has retired, per HTB's content policy.
{: .prompt-warning }

## Machine Info

- **Platform:** Hack The Box / TryHackMe
- **Difficulty:** Easy
- **OS:** Linux
- **IP:** 10.10.11.xxx

## Overview

One or two sentences summarizing the box: what tech it uses, and the rough
shape of the attack chain (foothold → user → root).

## Reconnaissance

```bash
nmap -sC -sV -oN nmap/initial.txt 10.10.11.xxx
```

Paste (trimmed) nmap output and note what stood out — open ports,
service versions, any hostnames to add to `/etc/hosts`.

## Enumeration

Walk through what you found while poking at each service:
web app structure, exposed files, interesting endpoints, leaked
credentials, etc. Screenshots or terminal output go here.

## Foothold

Describe the vulnerability (link the CVE if there is one) and how you
turned it into a shell. Include the exact payload/command you used.

```bash
# exploitation command / payload
```

## User Flag

How you moved from initial shell to a full user account —
credential reuse, SSH key, sudo misconfig, etc.

## Privilege Escalation

The path from user → root: SUID binaries, cron jobs, kernel exploits,
misconfigured services, whatever it was. Include the commands and
why they worked.

```bash
# privesc command
```

## Root Flag

Confirm root access and wrap up.

## Lessons Learned

A few bullets on what this box taught you — a technique, a tool, a
pattern you'll now check for on future boxes. This section is what
makes a writeup useful to *you* later, not just to readers.
