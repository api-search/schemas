---
description: RevenueSnapshot schema from Aramark Marko API
layout: schema
name: RevenueSnapshot
properties_list:
- description: Profit center identifier
  name: profitCenterId
  type: string
- description: Revenue period (YYYY-MM)
  name: period
  type: string
- description: Total revenue for the period in USD
  name: totalRevenue
  type: number
- description: Number of transactions in the period
  name: transactionCount
  type: integer
- description: Average transaction value in USD
  name: averageTicket
  type: number
provider_name: Aramark
provider_slug: aramark
schema_file: json-schema/marko-api-revenue-snapshot-schema.json
slug: marko-api-revenue-snapshot
tags:
- Food Services
- Facilities Management
- Uniform Services
- Data Platform
- Fortune 500
title: RevenueSnapshot
---
