---
description: Party schema from Avalara API
layout: schema
name: Party
properties_list:
- description: ''
  name: name
  type: string
- description: Tax identification number
  name: identifier
  type: string
- description: Identifier scheme (e.g., VAT)
  name: identifierScheme
  type: string
- description: ''
  name: address
  type: object
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/e-invoicing-party-schema.json
slug: e-invoicing-party
tags:
- Taxes
title: Party
---
