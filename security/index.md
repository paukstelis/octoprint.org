---
layout: page
title: Security Policy
lastupdate: 2022-11-16 15:45:00 +0100
---

**If you think that you have found a security vulnerability in OctoPrint, please disclose it to us via our security e-mail address at [security@octoprint.org](mailto:security@octoprint.org) or via a [GitHub Security Advisory](https://github.com/OctoPrint/OctoPrint/security/advisories).**

We are mostly interested in reports by actual OctoPrint users that are familiar with the platform, but all high quality contributions are welcome. Please do your best to describe a clear and realistic impact for your report.

For the sake of OctoPrint's user base, **do not make vulnerabilities public without notifying us and giving us at least 90 days to release a fixed version**. We will do our best to respond to your report within 7 days, and also to keep you informed of the progress of our efforts to resolve the issue, but understand that OctoPrint like many Open Source projects is primarily a volunteer project with only one full-time resource, and we may not be able to respond as quickly as you would like due to other responsibilities.

If you are going to write about OctoPrint's security, please get in touch, so we can make sure that all claims are correct.

## Supported versions

We only accept reports against the latest stable & official version of OctoPrint or any versions beyond that currently in development (`maintenance`, `devel`, `staging/*`, `rc/*` branches on the Git repository). The latest version can be found [here](https://github.com/OctoPrint/OctoPrint/releases/latest).

We do not accept reports against forks of OctoPrint.

## Non-qualifying vulnerabilities

We will not accept reports of vulnerabilities of the following types:

- Reports from automated tools or scanners
- Theoretical attacks without proof of exploitability
- Attacks that are the result of a third party library (these should instead be reported to the library maintainers)
- Social engineering
- Attacks involving physical access to a user's device, or involving a device or network that's already seriously compromised (eg man-in-the-middle).
- Attacks that require the user to install a malicious plugin
- Attacks that require the user to install a malicious language pack
- Attacks that require the user to expose their OctoPrint instance on the public internet or another hostile network
- Attacks that the user can only perform on themselves

## Severity scoring

If you are familiar with [CVSS3.1](https://www.first.org/cvss/v3.1/specification-document), then please provide the score of the vulnerability in your report in the shape of a vector string. There's a calculator [here](https://www.first.org/cvss/calculator/3.1). If you are not sure how or unable to score a vulnerability, state that in your report and we will look into it.

If you intend to provide a score yourself, please make yourself familiar with CVSS *first* (we strongly recommend reading [Specification](https://www.first.org/cvss/v3.1/specification-document) and [Scoring Guide](https://www.first.org/cvss/v3.1/user-guide#Scoring-Guide)), as we will not accept reports that use it incorrectly.

When scoring Attack Vector, use `Adjacent` as a maximum. OctoPrint is supposed to be deployed in a secure private network. Deployments on the public internet or other hostile networks are considered a severe misconfiguration, not the default deployment scenario. We also stress this point in several places in the FAQ and OctoPrint itself.

## Public disclosure & CVE assignment

We will publish GitHub Security Advisories, and through those will also request CVEs, for valid vulnerabilities that meet the following criteria:

- The vulnerability is in OctoPrint itself, not a third party library
- The vulnerability is not already known to us
- The vulnerability is not already known to the public

CVEs will only be requested for vulnerabilities with a severity of Medium or higher.

## Bounties

As a crowd-funded community project, OctoPrint is not able to offer bounties for security vulnerabilities. However, if so desired we will give credit to the discoverer of a vulnerability in our release notes and the release announcements on the blog.

---

<center><em>This document was last updated on {{ page.lastupdate | date: "%B %-d, %Y" }}.</em></center>
