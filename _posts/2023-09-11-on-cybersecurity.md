---
# layout: post
title:  "On Cybersecurity"
date:   2023-09-11 16:55:00 -0600
categories: cybersecurity compliance monitoring backups risk severity encryption
---
## Summary
The world is growing evermore connected. Cybersecurity best practices should be in the to-do list, periodically reviewed, and acted upon. There is always room for improvement.

## Segregated Environments
* Development: testing and development done here
* Staging: integration testing, rollback testing, preparing for Prod deploy
* Production: necessarily rigid
* Environmental alignment and Hydration

## Access Control Lists - Who can do What Where and When?
* Deployment Environments: dev, stage, prod
* Applications: Who has access to the infrastructure or intellectual property?
* Backups - who has access to the backups, what can they do, and when?

## Encryption - Sensitive Data
* HTTPS everywhere - it is silly not to have this in place now
* Production - Database and Data stores
* Backups - all data at rest
* PII/SPII content
* Are the credentials for decryption secure? See access control lists

## Monitoring
* What metrics/thresholds matter? "Do we care if the CPU is above 80%? What about 50%? Disk Space? HTTP sockets?"
* Do we have level-1 response runbooks? "What does level-1 do if this alert happens?"
* Do we have escalation paths? "If level-1 doesn't respond in N minutes..."
* What logs/metrics are piped where? DataDog, Splunk/SumoLogic, PagerDuty (system metrics, system logs, application logs, access logs, audit logs, event logs, service logs, etc.)

## Software Patching
* Automate all the small stuff (minor kernel patches and restarts)
* Schedule the big stuff in accordance with infrastructure and service-level agreements
* Keep all the software as up-to-date as possible to reduce likelihood of old exploits existing in the product.

## Vulnerability Scanning / Assessments
* Compare current versions with disclosed or known vulnerabilities and libraries
* Make a Risk, Likelihood, and Severity assessment matrix
* Make Remediation assessments: how much risk is involved, how much work does it take to implement, what is the ROI on that?
