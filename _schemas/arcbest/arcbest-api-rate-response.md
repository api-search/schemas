---
description: ''
layout: schema
name: RateResponse
properties_list:
- description: Quote reference number
  name: quoteNumber
  type: string
- description: Total freight charge in USD
  name: totalCharge
  type: number
- description: Estimated transit days
  name: transitDays
  type: integer
- description: Service level
  name: serviceLevel
  type: string
- description: Quote expiration timestamp
  name: expiresAt
  type: string
provider_name: ArcBest
provider_slug: arcbest
schema_file: json-schema/arcbest-api-rate-response-schema.json
slug: arcbest-api-rate-response
tags:
- Logistics
- Freight
- LTL
- Supply Chain
- Shipping
- Transportation
title: RateResponse
---
