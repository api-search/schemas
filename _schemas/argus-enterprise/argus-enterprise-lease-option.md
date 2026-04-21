---
description: LeaseOption schema from ARGUS Enterprise API
layout: schema
name: LeaseOption
properties_list:
- description: Type of lease option
  name: optionType
  type: string
- description: Date by which notice must be given
  name: noticeDate
  type: string
- description: Date the option can be exercised
  name: exerciseDate
  type: string
- description: Duration of option term in months
  name: termMonths
  type: integer
- description: Description of rent adjustment terms
  name: rentAdjustment
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-lease-option-schema.json
slug: argus-enterprise-lease-option
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: LeaseOption
---
