---
description: Tenant schema from ARGUS Enterprise API
layout: schema
name: Tenant
properties_list:
- description: Unique tenant identifier
  name: id
  type: string
- description: Tenant company or individual name
  name: name
  type: string
- description: Tenant industry classification
  name: industry
  type: string
- description: Tenant credit rating
  name: creditRating
  type: string
- description: Primary contact name
  name: contactName
  type: string
- description: Primary contact email
  name: contactEmail
  type: string
- description: Primary contact phone
  name: contactPhone
  type: string
- description: ''
  name: address
  type: object
- description: Number of active leases
  name: activeLeases
  type: integer
- description: Total leased area across all properties
  name: totalLeasedArea
  type: number
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-tenant-schema.json
slug: argus-enterprise-tenant
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: Tenant
---
