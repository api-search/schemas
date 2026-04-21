---
description: Represents a property valuation in the ARGUS Enterprise platform, capturing DCF analysis, direct capitalization, or comparable sales methodology results including key financial metrics.
layout: schema
name: Argus Enterprise Valuation
properties_list:
- description: Unique valuation identifier
  name: id
  type: string
- description: Associated property identifier
  name: propertyId
  type: string
- description: Date of valuation
  name: valuationDate
  type: string
- description: Valuation methodology used
  name: methodology
  type: string
- description: Estimated market value
  name: marketValue
  type: number
- description: Capitalization rate (percentage)
  name: capRate
  type: number
- description: Discount rate used in DCF analysis (percentage)
  name: discountRate
  type: number
- description: Terminal capitalization rate for DCF analysis (percentage)
  name: terminalCapRate
  type: number
- description: Start date of the analysis period
  name: analysisStartDate
  type: string
- description: End date of the analysis period
  name: analysisEndDate
  type: string
- description: Stabilized net operating income
  name: netOperatingIncome
  type: number
- description: Net present value from DCF analysis
  name: netPresentValue
  type: number
- description: Internal rate of return (percentage)
  name: internalRateOfReturn
  type: number
- description: Currency code (ISO 4217)
  name: currency
  type: string
- description: Additional notes or assumptions
  name: notes
  type: string
- description: Username of the creator
  name: createdBy
  type: string
- description: Record creation timestamp
  name: createdAt
  type: string
- description: Record last update timestamp
  name: updatedAt
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-valuation-schema.json
slug: argus-enterprise-valuation
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: Argus Enterprise Valuation
---
