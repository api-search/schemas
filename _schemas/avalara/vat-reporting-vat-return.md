---
description: VATReturn schema from Avalara API
layout: schema
name: VATReturn
properties_list:
- description: ''
  name: returnId
  type: string
- description: ''
  name: companyId
  type: string
- description: ISO 3166-1 alpha-2 country code
  name: countryCode
  type: string
- description: ''
  name: vatRegistrationNumber
  type: string
- description: ''
  name: returnType
  type: string
- description: ''
  name: periodStart
  type: string
- description: ''
  name: periodEnd
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: totalOutputVAT
  type: number
- description: ''
  name: totalInputVAT
  type: number
- description: ''
  name: netVATDue
  type: number
- description: ''
  name: submissionDate
  type: string
- description: ''
  name: currency
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/vat-reporting-vat-return-schema.json
slug: vat-reporting-vat-return
tags:
- Taxes
title: VATReturn
---
