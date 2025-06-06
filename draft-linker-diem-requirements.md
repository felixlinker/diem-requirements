---
title: "DIEM Use Cases and Requirements"
category: info

docname: draft-linker-diem-requirements-latest
submissiontype: IETF  # also: "independent", "editorial", "IAB", or "IRTF"
number:
date:
consensus: true
v: 3
area: "Applications and Real-Time"
workgroup: "Digital Emblems"
keyword:
 - next generation
 - unicorn
 - sparkling distributed ledger
venue:
  group: "Digital Emblems"
  type: "Working Group"
  mail: "diem@ietf.org"
  arch: "https://mailarchive.ietf.org/arch/browse/diem"
  github: "felixlinker/diem-requirements"
  latest: "https://felixlinker.github.io/diem-requirements/draft-linker-diem-requirements.html"

author:
 -
    fullname: Felix Linker
    email: linkerfelix@gmail.com

normative:

informative:

...

--- abstract

TODO Abstract


--- middle

# Introduction

TODO Introduction


# Conventions and Definitions

{::boilerplate bcp14-tagged}

# Use Cases and Requirements for Initial Scope

## Use Cases

### Digital Emblems under International Humanitarian Law

The Geneva Conventions and their *Additional Protocols* (APs) constitute the core of International Humanitarian Law (IHL) and establish legal rules on the conduct of armed conflict.
They codify four types of protective emblems, which inform other parties that assets bearing them must not be attacked:

- The emblems of the Red Cross, Red Crystal, and Red Crescent is applied to assets that undertake medical functions.
- The Blue Shield emblem to identify cultural property.
- The emblem for the protection of civil defense.
- The emblem to identify objects containing dangerous forces, i.e., whose destruction can release dangerous forces.

Digital emblems under IHL MUST identify the issuing party and MUST provide a means for authorization by third parties.

## Requirements

### Authenticity

Validators MUST be able to verify that an emblem was issued for the respective bearer, issued by the claimed issuer (where applicable), and that none of its associated data was changed.

Use cases that have this requirement:
- Emblems under IHL

### Issuance and Authorization

Validators MUST be able to verify that an emblem issuer was authorized to issue the emblem.
Authorizing parties MAY limit what emblems an issuer can issue, e.g., they MAY limit issuance to certain bearers.

Use cases that have this requirement:
- Emblems under IHL

#### Decentralization

Anyone MUST be able to authorize an issuer.

Use cases that have this requirement:
- Emblems under IHL

#### Accountability

Emblem issuance and authorization of issuers MUST be attributable to issuers and authorizing parties.
Authorizing parties and emblem issuers MUST NOT be able to repudiate that they issued an emblem or authorization.

Use cases that have this requirement:
- Emblems under IHL

#### Revocation

Emblems and authorizations MUST be revokable within reasonable windows of time.
Depending on the design, it may suffice to rely on expiration of short-lived emblems and authorization effectively as a revocation mechanism.

Use cases that have this requirement:
- Emblems under IHL

### Covert Inspection

Emblem issuers MUST NOT be able to detect whether someone is requesting or validating emblems issued by them.

Use cases that have this requirement:
- Emblems under IHL

# Other Use Cases and Requirements

## Use Cases

## Requirements

# Security Considerations

TODO Security


# IANA Considerations

This document has no IANA actions.


--- back

# Acknowledgments
{:numbered="false"}

TODO acknowledge.
