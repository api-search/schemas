---
description: ''
layout: schema
name: CommodityDetail
properties_list:
- description: Unique commodity identifier
  name: id
  type: string
- description: Commodity display name
  name: name
  type: string
- description: Commodity type
  name: type
  type: string
- description: Current market price
  name: currentPrice
  type: number
- description: Price currency
  name: currency
  type: string
- description: Price unit of measure
  name: unit
  type: string
- description: Date of price quote
  name: priceDate
  type: string
- description: 52-week high price
  name: weekHigh
  type: number
- description: 52-week low price
  name: weekLow
  type: number
- description: Daily trading volume in bushels
  name: volume
  type: integer
provider_name: Archer Daniels Midland
provider_slug: archer-daniels-midland
schema_file: json-schema/archer-daniels-midland-commodity-data-api-commodity-detail-schema.json
slug: archer-daniels-midland-commodity-data-api-commodity-detail
tags:
- Agriculture
- Food Processing
- Commodities
- Supply Chain
- Fortune 100
- Nutrition
title: CommodityDetail
---
