---
description: Invoice schema from Avalara API
layout: schema
name: Invoice
properties_list:
- description: Document code
  name: doc
  type: string
- description: Commit indicator
  name: cmmt
  type: boolean
- description: ''
  name: bill
  type: object
- description: Customer type
  name: cust
  type: integer
- description: Invoice date
  name: date
  type: string
- description: Line items on the invoice
  name: itms
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/communications-invoice-schema.json
slug: communications-invoice
tags:
- Taxes
title: Invoice
---
