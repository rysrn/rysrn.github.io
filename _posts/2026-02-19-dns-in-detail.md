---
title: "Lab Writeup: DNS in detail"
date: 2026-02-19 15:34:25 +0300
categories: [Cyber Security, Labs]
tags: [nmap, dns, tryhackme, writeup]
---

## 🚩 Introduction
Beyond simple name resolution, DNS is a critical protocol used for everything from email routing to domain ownership verification. This module breaks down common DNS record types (A, AAAA, MX, CNAME, and TXT) and explains how their settings, such as Time to Live (TTL), impact global network performance and security.

## 🛠️ Tools Used
All technical tools and platforms involved in the solution:
- **Platform:** TryHackMe (DNS in Detail Room)
- **Scanning:** `nslookup`
- **Operating System:** Kali Linux

## 🔍 Approach & Methodology
Break down your steps logically:
1.  **Enumeration:** I started by identifying the authoritative name servers for the domain.
2.  **Analysis:** I queried specific record types (A, MX, TXT) to find anomalies.
3.  **Discovery:** I found a non-standard record pointing to a hidden subdomain.

## 📸 Proof of Concept (Screenshots)
![DNS Query Results](assets/lab1.PNG)

## 💡 Key Lessons Learned
What I learnt.
- **DNS Hierarchy:** Deepened my understanding of how Recursive vs. Authoritative servers interact.
- **Command Efficiency:** Learned how to use `dig +short` for cleaner output during rapid assessments.
- **Persistence:** Realized that sometimes critical data is hidden in less common records like TXT or CNAME.
