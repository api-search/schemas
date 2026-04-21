---
description: A cost allocation record tracking technology spending in Apptio
layout: schema
name: CostAllocation
properties_list:
- description: Unique cost allocation identifier
  name: allocationId
  type: string
- description: Cost center or department receiving the allocation
  name: costCenter
  type: string
- description: Technology cost category (infrastructure, software, labor, etc.)
  name: category
  type: string
- description: Reporting period (YYYY-MM)
  name: period
  type: string
- description: Allocated cost amount in USD
  name: amount
  type: number
- description: Currency code
  name: currency
  type: string
- description: Technology vendor or provider
  name: vendor
  type: string
- description: Custom metadata tags for the allocation
  name: tags
  type: object
provider_name: Apptio
provider_slug: apptio
schema_file: json-schema/cost-allocation-schema.json
slug: cost-allocation
tags:
- Analytics
- Cost Management
- IT Finance
- Technology Business Management
title: CostAllocation
---
