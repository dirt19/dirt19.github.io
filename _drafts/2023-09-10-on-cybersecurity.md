---
# layout: post
title:  "On Cybersecurity"
date:   2023-09-10 15:00:00 -0600
categories: cybersecurity compliance monitoring backups risk severity encryption
---
## Summary
Sometimes in creating and using a tool, you become reliant upon it.

## Access Control Lists - Who can do What When?
* Development - who can access the lower environments and what can they do?
* Production - who can access the production environments and what can they do?
* Backups - who has access to the backups, what can they do, and when?

## Encryption - Sensitive Data
* HTTPS everywhere - it is silly not to have this in place now
* Production - Database and Data stores
* Backups - all data at rest or in 
* PII/SPII content
* Are the credentials for decryption secure? See access control lists

## Monitoring
* What metrics/thresholds matter? "Do we care if the CPU is above 80%? What about 50%? Disk Space? HTTP sockets?"
* Do we have level-1 response runbooks? "What does level-1 do if this alert happens?"
* Do we have escalation paths? "If level-1 doesn't respond in N minutes..."
* What logs/metrics are piped where? DataDog, Splunk/SumoLogic, PagerDuty (metrics, system logs, application logs, access logs, audit logs, event logs, service logs, etc.)

## Software Patching
* Automate all the small stuff (minor kernel patches and restarts)
* Schedule the big stuff in accordance with infrastructure and service-level agreements

## Vulnerability Scanning / Assessments
* Compare current versions with disclosed or known vulnerabilities and libraries
* Make a Risk, Likelihood, and Severity assessment
* Make Remediation assessments