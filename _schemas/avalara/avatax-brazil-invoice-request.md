---
description: InvoiceRequest schema from Avalara API
layout: schema
name: InvoiceRequest
properties_list:
- description: Electronic document type
  name: invoiceType
  type: string
- description: ''
  name: companyId
  type: string
- description: ''
  name: transactionDate
  type: string
- description: ''
  name: buyer
  type: object
- description: ''
  name: lines
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-brazil-invoice-request-schema.json
slug: avatax-brazil-invoice-request
tags:
- Taxes
title: InvoiceRequest
---
