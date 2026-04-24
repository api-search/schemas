---
description: Schema for a Blackstone alternative investment fund record
layout: schema
name: Blackstone Fund
properties_list:
- description: Unique fund identifier
  name: fundId
  type: string
- description: Full legal fund name
  name: fundName
  type: string
- description: Investment strategy
  name: strategy
  type: string
- description: Fund vintage year
  name: vintage
  type: integer
- description: Base currency (ISO 4217)
  name: currency
  type: string
- description: Total committed capital
  name: committedCapital
  type: number
- description: Capital called to date
  name: calledCapital
  type: number
- description: Net asset value
  name: nav
  type: number
- description: ''
  name: navDate
  type: string
- description: Internal rate of return
  name: irr
  type: number
- description: Multiple on invested capital
  name: moic
  type: number
- description: ''
  name: status
  type: string
provider_name: Blackstone
provider_slug: blackstone
schema_file: json-schema/blackstone-fund-schema.json
slug: blackstone-fund
tags:
- Alternative Assets
- Finance
- Investment Management
- Private Equity
- Real Estate
title: Blackstone Fund
---
