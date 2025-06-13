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

Use cases listed in the Section will not be addressed within the initial scope of DIEM.
They are listed here for documentation and future reference.
The requirements of these use cases are not complete and would need to be investigated further when addressing the use cases.

## Marking of Hazardous Materials

The Organization for the Prohibition of Chemical Weapons (OPCW), the Inrernational Atomic Energy Agency (IAEA), and the Basel Convention require that certain, dangerous materials are marked during shipment.
Concretely:

- The OPCW requires marking of Schedule 1 chemicals.
- The IAEA administers several treaties related to the shipment of atomic fuels and wasters across borders.
- The Basel Convention regulates the trans-boundary movement of hazardous wastes.

An emblem MUST provide a description, location, date, and quantity.
The description MUST be accessible only by authorized parties, e.g., customs agencies or material handlers.

## Marking of Brand-Associated Shipments

World Intellectual Property Organization (WIPO) administers treaters, in particular the Madrid Protocol, that allow brands to mark their shipments with an emblem so that customs agents can identify legitimate products.

An emblem MUST identify the copyright/brand image, provide a textual description of the shipment, and a chain-of-custody/provenance.

## Marking of Civil Aviation Flights

The International Civil Aviation Organization (ICAO) requires that civil aviation flights are protected and that one can verify them to not be dual-use (i.e., not carrying military cargo).

An emblem MUST carry a geographic description of the flight plan, its current location, and a textual description of the flight including its manifest, identifying characteristics, and its identity, e.g., tail number.
An emblem may need to also reference a flight manifest.

# Security Considerations

TODO Security


# IANA Considerations

This document has no IANA actions.


--- back

# Acknowledgments
{:numbered="false"}

TODO acknowledge.
