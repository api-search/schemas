---
description: Represents a commercial real estate property in the ARGUS Enterprise platform, including physical attributes, financial metrics, and portfolio association.
layout: schema
name: Argus Enterprise Property
properties_list:
- description: Unique property identifier
  name: id
  type: string
- description: Property name
  name: name
  type: string
- description: Type of commercial real estate property
  name: propertyType
  type: string
- description: Current property status
  name: status
  type: string
- description: Property physical address
  name: address
  type: object
- description: Gross leasable area in square feet
  name: grossArea
  type: number
- description: Net leasable area in square feet
  name: netLeasableArea
  type: number
- description: Year the property was built
  name: yearBuilt
  type: integer
- description: Number of leasable units or suites
  name: numberOfUnits
  type: integer
- description: Original purchase price
  name: purchasePrice
  type: number
- description: Date of property acquisition
  name: purchaseDate
  type: string
- description: Current estimated market value
  name: currentMarketValue
  type: number
- description: Current occupancy rate as a percentage
  name: occupancyRate
  type: number
- description: Identifier of the parent portfolio
  name: portfolioId
  type: string
- description: Record creation timestamp
  name: createdAt
  type: string
- description: Record last update timestamp
  name: updatedAt
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-property-schema.json
slug: argus-enterprise-property
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: Argus Enterprise Property
---
