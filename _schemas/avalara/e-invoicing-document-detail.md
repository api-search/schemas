---
description: DocumentDetail schema from Avalara API
layout: schema
name: DocumentDetail
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: dataFormat
  type: string
- description: ''
  name: documentType
  type: string
- description: ''
  name: invoiceNumber
  type: string
- description: ''
  name: invoiceDate
  type: string
- description: ''
  name: sender
  type: object
- description: ''
  name: recipient
  type: object
- description: ''
  name: totalAmount
  type: number
- description: ''
  name: currencyCode
  type: string
- description: ''
  name: countryCode
  type: string
- description: ''
  name: submissionDate
  type: string
- description: ''
  name: events
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/e-invoicing-document-detail-schema.json
slug: e-invoicing-document-detail
tags:
- Taxes
title: DocumentDetail
---
