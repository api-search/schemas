---
description: ''
layout: schema
name: UpdateCustomSymbolTypeDto
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: hideAddressField
  type: boolean
- description: ''
  name: hideSymbolSubtype
  type: boolean
- description: ''
  name: isDefault
  type: boolean
- description: ''
  name: subTypes
  type: array
- description: ''
  name: customFieldIds
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-irn-configuration-update-custom-symbol-type-dto-schema.json
slug: factset-irn-configuration-update-custom-symbol-type-dto
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateCustomSymbolTypeDto\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"hideAddressField\": {\n      \"type\": \"boolean\"\n    },\n    \"hideSymbolSubtype\": {\n      \"type\": \"boolean\"\n    },\n    \"isDefault\": {\n      \"type\": \"boolean\"\n    },\n    \"subTypes\": {\n      \"type\": \"array\"\n    },\n    \"customFieldIds\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-irn-configuration-update-custom-symbol-type-dto-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: UpdateCustomSymbolTypeDto
---
