---
description: CashFlowProjection schema from ARGUS Enterprise API
layout: schema
name: CashFlowProjection
properties_list:
- description: Associated property identifier
  name: propertyId
  type: string
- description: Projection start date
  name: startDate
  type: string
- description: Projection end date
  name: endDate
  type: string
- description: Cash flow reporting frequency
  name: frequency
  type: string
- description: Currency code (ISO 4217)
  name: currency
  type: string
- description: Individual cash flow periods
  name: periods
  type: array
- description: ''
  name: summary
  type: object
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-cash-flow-projection-schema.json
slug: argus-enterprise-cash-flow-projection
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: CashFlowProjection
---
