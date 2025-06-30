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

The Digital Emblems (DIEM) working group (WG) will define an architecture and discovery mechanism to present and validate digital emblems.
This document lists use cases for the current and future scope of the DIEM WG and their associated requirements.

--- middle

# Introduction

The Digital Emblems (DIEM) working group (WG) will define an architecture and discovery mechanism to present and validate digital emblems.
Digital emblems extend the range of existing, identifying marks (for examples, see the use cases below) from the physical (visual and tactile) to the digital realm.
This document lists use cases for the current and future scope of the DIEM WG and their associated requirements.
As of writing, the DIEM has an initial scope that limits WG work to digital emblems that can be discovered using the DNS and that identify their bearer by a Fully Qualified Domain Name (FQDN).
The WG intends to address use cases presented in {{uc-initial}} within the WG's initial scope, and presents use cases in {{uc-other}} for future WG work and reference.

# Conventions and Definitions

{::boilerplate bcp14-tagged}

# Use Cases and Requirements for Initial Scope {#uc-initial}

Below listed use cases are intended to be addressed within the DIEM WG's initial scope (as chartered as of writing).
Every use case lists its associated requirements, which are specified in {{reqs}}.

## Digital Emblems under International Humanitarian Law

The Geneva Conventions and their Additional Protocols constitute the core of International Humanitarian Law (IHL) and establish legal rules on the conduct of armed conflict.
Some assets enjoy certain specific protections under IHL, including that they must not be attacked, and IHL codifies four types of protective emblems for armed conflict, which inform other parties that marked assets benefit from one or several of these specific protections.
Note that assets enjoy there protections irrespective of whether they are marked with the respective emblem.
The emblem only serves to inform others of these protections.

- The emblems of the Red Cross, Red Crescent, and Red Crystal are applied to assets of the medical services as well as the assets of certain humanitarian operations.
- The Blue Shield emblem is applied to cultural property.
- The emblem for the protection of civil defense is applied to certain assets for the protection of the civilian population against the dangers of hostilities or disasters.
- The dangerous forces emblem is applied to works or installations containing dangerous forces, i.e., dams, dikes, and nuclear generating facilities.

Digital emblems under IHL will be borne by network-connected and network-addressable assets that enjoy aforementioned specific protections under IHL and whose disruption would violate these protections.

### Requirements

Digital emblems under IHL MUST identify the issuing party and MUST provide a means for authorization by third parties.
Additionally, this use case has the following requirements:

- Authenticity
- Authorization and Decentralized Authorization
- Accountability
- Revocation
- Undetectable Validation

## Marking of the Press

TODO

## The Ramsar Convention

TODO

# Other Use Cases and Requirements {#uc-other}

The initial DIEM efforts do not include the following use cases.
They are listed here for documentation and future reference.
The requirements of these use cases are not complete and would need to be investigated further when addressing the use cases.

## Marking of Hazardous Materials

The Organization for the Prohibition of Chemical Weapons (OPCW), the International Atomic Energy Agency (IAEA), and the Basel Convention require that certain, dangerous materials are marked during shipment.
Concretely:

- The OPCW requires marking of Schedule 1 chemicals.
- The IAEA administers several treaties related to the shipment of atomic fuels and wasters across borders.
- The Basel Convention regulates the trans-boundary movement of hazardous wastes.

An emblem MUST provide a description, location, date, and quantity.
The description MUST be accessible only by authorized parties, e.g., customs agencies or material handlers.

## Marking of Brand-Associated Shipments

World Intellectual Property Organization (WIPO) administers treaties, in particular the Madrid Protocol, that allow brands to mark their shipments with an emblem so that customs agents can identify legitimate products.

An emblem MUST identify the copyright/brand image, provide a textual description of the shipment, and a chain-of-custody/provenance.

## Marking of Civil Aviation Flights

The International Civil Aviation Organization (ICAO) requires that civil aviation flights are protected and that one can verify them to not be dual-use, e.g., not carrying military cargo.

An emblem MUST carry a geographic description of the flight plan, its current location, and a textual description of the flight including its manifest, identifying characteristics, e.g., tail number.
An emblem may need to also reference a flight manifest.

# Requirements {#reqs}

## Authenticity

Validators MUST be able to verify that an emblem was issued for the respective bearer, issued by the claimed issuer (where applicable), and that none of its associated data was changed.

## Authorization

Validators MUST be able to verify that an emblem issuer was authorized to issue the emblem.
Authorizing parties MAY limit what emblems an issuer can issue, e.g., they MAY limit issuance to certain bearers.

### Decentralized Authorization

Anyone MUST be able to authorize an issuer.

## Accountability

Emblem issuance and authorization of issuers (where applicable) MUST be attributable to issuers and authorizing parties.
Authorizing parties and emblem issuers MUST NOT be able to repudiate that they issued an emblem or authorization.

## Revocation

Emblems and authorizations (where applicable) MUST be revokable within reasonable windows of time.
Depending on the design, it may suffice to rely on expiration of short-lived emblems and authorization effectively as a revocation mechanism.

## Undetectable Validation

Bearers MUST NOT be able to detect whether someone is requesting or validating emblems issued for them.

## Visual

An emblem MUST be capable of carrying a visual representation of the physical emblem it represents.

## Law Carrying

An emblem MUST carry an unambiguous indication of the international law or laws conferring the semantics of the emblem.

## Proximity-Based Distribution

An emblem MUST be presentable using an in-band, proximity-based protocol such as a QR code or RFID.

## Physical Binding

An emblem MUST be possible to associate with physical assets, e.g., buildings, vehicles, or containers.

### Quantifiable

An emblem MUST be possible to associate with a range or specific quantity of associated, physical assets.

### Geographic

An emblem MUST be restrictable by geographic scope.

## Identity Binding

An emblem MUST be possible to associate with a person or group of people.

## Human-Readable Validation Data

An emblem MUST be capable of providing additional relevant information (e.g., photographs, unique identifiers) which can be used to corroborate the association of the digital emblem with the entity bearing it.

# Security Considerations

TODO Security


# IANA Considerations

This document has no IANA actions.

# Contributors

Parts of this document are based on {{?I-D.draft-haberman-digital-emblem-ps-03}} and {{?I-D.draft-linker-digital-emblem-02}}.
As part of that, Brian Haberman (brian@innovationslab.net), Tommy Jensen (tojens@microsoft.com), and Bill Woodcock (woody@pch.net) contributed to writing this document.
Furhermore, Rohan Mahy (rohan.ietf@gmail.com) provided valuable feedback on contents and structure, and Samit D'Cunha (sdcunha@icrc.org) provided feedback on the IHL aspects of this document.

--- back

# Acknowledgments
{:numbered="false"}

TODO acknowledge.
