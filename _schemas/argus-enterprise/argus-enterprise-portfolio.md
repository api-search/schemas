---
description: Represents a commercial real estate portfolio in the ARGUS Enterprise platform, used to organize and manage groups of properties under a unified investment strategy.
layout: schema
name: Argus Enterprise Portfolio
properties_list:
- description: Unique portfolio identifier
  name: id
  type: string
- description: Portfolio name
  name: name
  type: string
- description: Portfolio description
  name: description
  type: string
- description: Investment strategy classification
  name: strategy
  type: string
- description: Number of properties in the portfolio
  name: totalProperties
  type: integer
- description: Aggregate market value of all properties
  name: totalMarketValue
  type: number
- description: Currency code (ISO 4217)
  name: currency
  type: string
- description: Record creation timestamp
  name: createdAt
  type: string
- description: Record last update timestamp
  name: updatedAt
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-portfolio-schema.json
slug: argus-enterprise-portfolio
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: Argus Enterprise Portfolio
---
