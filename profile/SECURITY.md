# Vulnerability Disclosure Policy & Bug Bounty Program

_Last updated: September 5, 2026_

## Introduction

PrivacySafe is a family of privacy and security software, public-interest services, protocols, and infrastructure supported by PrivacySafe Foundation, Inc. and commercially published and supported by Ivy Cyber LLC. We welcome good-faith security research that helps us protect users, software, public services, and infrastructure.

PrivacySafe Foundation publishes the public security scope and vulnerability-disclosure policy. Ivy Cyber provides technical security operations, triage, remediation coordination, infrastructure support, and, where applicable, bug-bounty administration for PrivacySafe systems.

We build on Free/Libre and Open Source Software (FLOSS) and favor responsible disclosure, reproducible reports, and transparent remediation.

## Open Bug Bounty

Our program is listed at [Open Bug Bounty](https://www.openbugbounty.org/bugbounty/privacysafe/). Submit there when feasible, or use the official encrypted reporting channel below.

## Scope

This policy applies to current PrivacySafe source repositories and public-facing systems maintained by PrivacySafe Foundation or administered for PrivacySafe projects by Ivy Cyber, including:

- `privacysafe.foundation`
- `privacysafe.app`
- `download.privacysafe.app`
- `privacysafe.social`
- `privacysafe.is`
- `privacysafe.bot`
- `privacysafe.locker`
- `psafe.ly`
- current PrivacySafe repositories at [github.com/PrivacySafe](https://github.com/PrivacySafe) and [codeberg.org/PrivacySafe](https://codeberg.org/PrivacySafe)
- other systems explicitly identified as in scope by a repository, service, or published security notice

### Out of scope

Unless we explicitly say otherwise, this policy does not authorize testing of:

- archived repositories;
- third-party services, federated servers, hosting providers, payment processors, or infrastructure we do not control;
- social engineering of users, staff, contributors, donors, customers, or partners;
- physical facilities, devices, or data centers not owned or controlled by us;
- denial-of-service or resource-exhaustion testing;
- destructive testing or testing that risks another person's data;
- public support, marketing, or social-media accounts as attack targets; or
- commonplace reports listed below without a demonstrated security impact specific to our implementation.

If you discover an issue in a third-party service, report it to that service's operator rather than testing it through our users or systems.

## Contact

### Non-security help

For ordinary help or non-sensitive issues that are not security or privacy vulnerabilities, contact:

`help@privacysafe.net`

GPG fingerprint:

`7702 BD22 435B 5F3E B00C 1E78 21FB 9DF4 D742 422D`

Verify the key through [keys.openpgp.org](https://keys.openpgp.org/search?q=help%40privacysafe.net).

Do not send passwords, recovery phrases, private keys, full payment credentials, or other secrets through ordinary email.

### Security issues

Report vulnerabilities, exploits, exposed data, privacy failures, and suspected breaches to:

`security@privacysafe.net`

GPG fingerprint:

`7E3E C7D6 D965 CF1D 8C76 8F80 74AB DBE3 E3FB C689`

Verify the key through [keys.openpgp.org](https://keys.openpgp.org/search?q=security%40privacysafe.net).

Our canonical `security.txt` is published at [privacysafe.app/security.txt](https://privacysafe.app/security.txt).

If you need to send sensitive material, encrypt it to the security key before transmission. If you use a paste service, encrypt the content first and send only the encrypted material.

## What a useful report includes

A security report should include:

- a clear description of the issue;
- the affected service, repository, version, endpoint, or build;
- steps to reproduce the issue;
- a proof of concept when safe;
- the expected and actual behavior;
- your assessment of security or privacy impact; and
- screenshots, video, logs, or other evidence when useful.

If you know a practical mitigation, include it. Do not access more data than necessary to demonstrate the issue.

## Our commitments

For reports that follow this policy, we will try to:

- acknowledge the report promptly;
- validate and triage it with the reporter;
- communicate whether it appears eligible for a bounty within five business days;
- keep the reporter reasonably informed while remediation is underway;
- remediate validated issues according to severity and operational constraints; and
- provide a disclosure window after a fix is deployed.

We use a coordinated disclosure period of up to 90 days unless the parties agree otherwise or urgent circumstances require a different timeline.

## Researcher expectations

When testing or reporting, you must:

- act in good faith;
- use only systems that are in scope;
- use accounts and data you own or have explicit permission to test;
- stop immediately if you encounter another user's private data;
- avoid disruption, persistence, destructive actions, privilege abuse, and denial-of-service;
- avoid social engineering;
- keep vulnerability details confidential until the coordinated disclosure window ends or we approve disclosure; and
- comply with applicable law.

Do not use a vulnerability to access, download, alter, delete, deanonymize, or publish another person's data beyond the minimum strictly necessary to demonstrate the issue safely.

## Safe harbor

We consider research conducted in good faith and in accordance with this policy to be authorized by us with respect to systems we control. We will not initiate or support legal action for accidental, good-faith violations of this policy when the researcher promptly stops, reports the issue, and cooperates in remediation.

This safe harbor applies only to claims under the control of the organizations participating in this policy. It cannot bind independent third parties or excuse violations of law unrelated to authorized security research.

If you are unsure whether planned testing is allowed, contact `security@privacysafe.net` before proceeding.

## Bounty rewards

Rewards depend on severity, quality of the report, exploitability, impact, and whether the issue is already known.

- **Critical:** up to $500 USD or equivalent cryptocurrency
- **High:** up to $250 USD or equivalent cryptocurrency
- **Medium or Low:** merchandise, digital rewards, acknowledgements, recommendations, or other recognition at our discretion

A researcher may request that an approved monetary reward be donated to an eligible charitable organization instead.

Only the first complete report of a previously unknown issue is normally eligible for a monetary reward.

## Commonplace reports

The following generally do not qualify for a bounty unless the report demonstrates a concrete exploit or material privacy/security impact specific to our implementation:

- missing non-critical security headers;
- descriptive errors, banners, or public version information;
- public files such as `robots.txt`;
- outdated dependencies without a demonstrated exploitable path;
- automated scan output without a reproducible exploit;
- non-exploitable configuration observations;
- clickjacking without demonstrated impact;
- logout CSRF;
- CSRF on anonymous forms without demonstrated impact;
- self-XSS;
- missing cookie flags without demonstrated impact;
- username enumeration without an exploit chain;
- rate-limit or account-lockout policy preferences;
- generic SSL/TLS best-practice observations;
- mail configuration observations such as SPF, DKIM, or DMARC preferences;
- public login panels;
- autocomplete settings;
- password-policy preferences; or
- subdomain or DNS findings that do not demonstrate control, data exposure, or a viable exploit.

## Acknowledgements

Researchers who responsibly disclose valid findings may be listed on our [Security Acknowledgements](https://privacysafe.app/security-thanks) page with their permission.
