---
description: Mandate schema from Avalara API
layout: schema
name: Mandate
properties_list:
- description: ''
  name: mandateId
  type: string
- description: ISO 3166-1 alpha-2 country code
  name: countryCode
  type: string
- description: ''
  name: countryName
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: supportedDocumentTypes
  type: array
- description: ''
  name: inputFormats
  type: array
- description: ''
  name: workflowId
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/e-invoicing-mandate-schema.json
slug: e-invoicing-mandate
tags:
- Taxes
title: Mandate
---
