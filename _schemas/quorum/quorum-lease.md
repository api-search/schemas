---
description: Schema for a Quorum Land Management oil and gas lease record representing a mineral rights agreement between a lessor and lessee.
layout: schema
name: Quorum Oil & Gas Lease
properties_list:
- description: Quorum system-generated lease identifier
  name: leaseId
  type: string
- description: Lease name or description
  name: leaseName
  type: string
- description: User-defined lease number
  name: leaseNumber
  type: string
- description: Current lease status
  name: status
  type: string
- description: Lease commencement/effective date
  name: effectiveDate
  type: string
- description: Lease expiration date; null if held by production
  name: expirationDate
  type:
  - string
  - 'null'
- description: Primary term duration in months
  name: primaryTerm
  type: integer
- description: Royalty rate as decimal fraction (e.g., 0.1875 = 18.75%)
  name: royaltyRate
  type: number
- description: Net mineral acres held under this lease
  name: netAcres
  type: number
- description: Gross acres in the lease
  name: grossAcres
  type: number
- description: County where the lease is located
  name: county
  type: string
- description: US state abbreviation (e.g., TX, OK, ND)
  name: state
  type: string
- description: Mineral rights owner / grantor name
  name: lessor
  type: string
- description: Oil company / operator holding the lease
  name: lessee
  type: string
- description: True if lease is currently held by production
  name: hbpStatus
  type: boolean
- description: True if deep rights are reserved from lease
  name: deepRightsReserved
  type: boolean
- description: True if surface waiver has been obtained
  name: surfaceWaiverObtained
  type: boolean
- description: ''
  name: createDatetime
  type: string
- description: ''
  name: lastUpdateDatetime
  type: string
provider_name: Quorum Software
provider_slug: quorum
schema_file: json-schema/quorum-lease-schema.json
slug: quorum-lease
source_filename: quorum-lease-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/quorum/json-schema/quorum-lease-schema.json\",\n  \"title\": \"Quorum Oil & Gas Lease\",\n  \"description\": \"Schema for a Quorum Land Management oil and gas lease record representing a mineral rights agreement between a lessor and lessee.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"leaseId\": {\n      \"type\": \"string\",\n      \"description\": \"Quorum system-generated lease identifier\"\n    },\n    \"leaseName\": {\n      \"type\": \"string\",\n      \"description\": \"Lease name or description\"\n    },\n    \"leaseNumber\": {\n      \"type\": \"string\",\n      \"description\": \"User-defined lease number\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"ACTIVE\", \"EXPIRED\", \"SURRENDERED\", \"HELD_BY_PRODUCTION\", \"PRODUCING\", \"SHUT_IN\"],\n      \"description\": \"Current lease status\"\n    },\n    \"effectiveDate\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Lease commencement/effective date\"\n    },\n    \"expirationDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Lease expiration date; null if held by production\"\n    },\n    \"primaryTerm\": {\n      \"type\": \"integer\",\n      \"description\": \"Primary term duration in months\"\n    },\n    \"royaltyRate\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 1,\n      \"description\": \"Royalty rate as decimal fraction (e.g., 0.1875 = 18.75%)\"\n    },\n    \"netAcres\": {\n      \"type\": \"number\",\n      \"description\": \"Net mineral acres held under this lease\"\n    },\n    \"grossAcres\": {\n      \"type\": \"number\",\n      \"description\": \"Gross acres in the lease\"\n    },\n    \"county\": {\n      \"type\": \"string\",\n      \"description\": \"County where the lease is located\"\n    },\n    \"state\"\
  : {\n      \"type\": \"string\",\n      \"maxLength\": 2,\n      \"description\": \"US state abbreviation (e.g., TX, OK, ND)\"\n    },\n    \"lessor\": {\n      \"type\": \"string\",\n      \"description\": \"Mineral rights owner / grantor name\"\n    },\n    \"lessee\": {\n      \"type\": \"string\",\n      \"description\": \"Oil company / operator holding the lease\"\n    },\n    \"hbpStatus\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if lease is currently held by production\"\n    },\n    \"deepRightsReserved\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if deep rights are reserved from lease\"\n    },\n    \"surfaceWaiverObtained\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if surface waiver has been obtained\"\n    },\n    \"createDatetime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"lastUpdateDatetime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n\
  \  \"required\": [\"leaseId\", \"leaseName\", \"status\", \"effectiveDate\", \"royaltyRate\", \"netAcres\", \"county\", \"state\", \"lessor\"],\n  \"examples\": [\n    {\n      \"leaseId\": \"LEASE-TX-001234\",\n      \"leaseName\": \"Smith Family Minerals\",\n      \"leaseNumber\": \"TX-001234\",\n      \"status\": \"PRODUCING\",\n      \"effectiveDate\": \"2022-05-01\",\n      \"expirationDate\": null,\n      \"primaryTerm\": 36,\n      \"royaltyRate\": 0.25,\n      \"netAcres\": 320.0,\n      \"grossAcres\": 640.0,\n      \"county\": \"Midland\",\n      \"state\": \"TX\",\n      \"lessor\": \"Smith Family Trust\",\n      \"lessee\": \"Acme Exploration LLC\",\n      \"hbpStatus\": true,\n      \"deepRightsReserved\": false,\n      \"surfaceWaiverObtained\": true\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/quorum/refs/heads/main/json-schema/quorum-lease-schema.json
tags:
- Energy
- Oil & Gas
- Upstream
- Land Management
- Royalty Accounting
- Production Reporting
title: Quorum Oil & Gas Lease
---
