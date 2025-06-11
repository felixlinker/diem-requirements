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

## Requirements

# Other Use Cases and Requirements

## Use Cases

## Requirements

### Authenticity

Validators MUST be able to verify that an emblem was issued for the respective bearer, issued by the claimed issuer (where applicable), and that none of its associated data was changed.

Use cases that have this requirement:

### Authorization

Validators MUST be able to verify that an emblem issuer was authorized to issue the emblem.
Authorizing parties MAY limit what emblems an issuer can issue, e.g., they MAY limit issuance to certain bearers.

Use cases that have this requirement:

#### Decentralized Authorization

Anyone MUST be able to authorize an issuer.

Use cases that have this requirement:

### Accountability

Emblem issuance and authorization of issuers (where applicable) MUST be attributable to issuers and authorizing parties.
Authorizing parties and emblem issuers MUST NOT be able to repudiate that they issued an emblem or authorization.

Use cases that have this requirement:

#### Revocation

Emblems and authorizations MUST be revokable within reasonable windows of time.
Depending on the design, it may suffice to rely on expiration of short-lived emblems and authorization effectively as a revocation mechanism.

Use cases that have this requirement:

### Undetectable Validation

Emblem issuers MUST NOT be able to detect whether someone is requesting or validating emblems issued by them.

Use cases that have this requirement:

### Visual

An emblem MUST be capable of carrying a visual representation of the physical emblem it represents.

Use cases that have this requirement:

### Law Carrying

An emblem MUST carry an unambiguous indication of the international law or laws conferring the semantics of the emblem.

Use cases that have this requirement:

### Proximity-Based Distribution

An emblem MUST be presentable using an in-band, proximity-based protocol such as a QR code or RFID.

Use cases that have this requirement:

### Physical Binding

An emblem MUST be possible to associate with physical assets, e.g., buildings, vehicles, or containers.

Use cases that have this requirement:

#### Quantifiable

An emblem MUST be possible to associate with a range or specific quantity of associated, physical assets.

Use cases that have this requirement:

#### Geographic

An emblem MUST be restrictable by geographic scope.

Use cases that have this requirement:

### Identity Binding

An emblem MUST be possible to associate with a person or group of people.

Use cases that have this requirement:

### Human-Readable Validation Data

An emblem MUST be capable of providing additional relevant information (e.g., photographs, unique identifiers) which can be used to corroborate the association of the digital emblem with the entity bearing it.

Use cases that have this requirement:

# Security Considerations

TODO Security


# IANA Considerations

This document has no IANA actions.


--- back

# Acknowledgments
{:numbered="false"}

TODO acknowledge.
