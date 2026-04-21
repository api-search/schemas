---
description: TaxResult schema from Avalara API
layout: schema
name: TaxResult
properties_list:
- description: Billable flag
  name: bill
  type: boolean
- description: Compliance flag
  name: cmpl
  type: boolean
- description: Taxable measure
  name: tm
  type: number
- description: Calculation type
  name: calc
  type: integer
- description: Tax category
  name: cat
  type: string
- description: Category ID
  name: cid
  type: integer
- description: Tax name
  name: name
  type: string
- description: Exempt amount
  name: exm
  type: number
- description: Lines
  name: lns
  type: integer
- description: Minutes
  name: min
  type: number
- description: PCode
  name: pcd
  type: integer
- description: Tax rate
  name: rate
  type: number
- description: Surcharge flag
  name: sur
  type: boolean
- description: Tax amount
  name: tax
  type: number
- description: Tax level (Federal, State, County, Local)
  name: lvl
  type: integer
- description: Tax type ID
  name: tid
  type: integer
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/communications-tax-result-schema.json
slug: communications-tax-result
tags:
- Taxes
title: TaxResult
---
