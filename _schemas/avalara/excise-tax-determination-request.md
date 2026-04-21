---
description: TaxDeterminationRequest schema from Avalara API
layout: schema
name: TaxDeterminationRequest
properties_list:
- description: Date for tax determination
  name: effectiveDate
  type: string
- description: ''
  name: invoiceNumber
  type: string
- description: ''
  name: invoiceDate
  type: string
- description: Title transfer point
  name: titleTransferCode
  type: string
- description: Type of excise transaction
  name: transactionType
  type: string
- description: ''
  name: seller
  type: object
- description: ''
  name: buyer
  type: object
- description: ''
  name: transactionLines
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/excise-tax-determination-request-schema.json
slug: excise-tax-determination-request
tags:
- Taxes
title: TaxDeterminationRequest
---
