---
description: ''
layout: schema
name: CreateCustomSymbolCustomFieldDto
properties_list:
- description: ''
  name: code
  type: string
- description: ''
  name: name
  type: string
- description: Type can be one of Text, SingleOption, MultiOptions, Numeric, Date, ExtendedText, ContactLookup
  name: type
  type: string
- description: ''
  name: isHidden
  type: boolean
- description: ''
  name: isMandatory
  type: boolean
- description: ''
  name: isShownInInfobox
  type: boolean
- description: ''
  name: optionsConfig
  type: array
- description: ''
  name: customSymbolTypes
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-irn-configuration-create-custom-symbol-custom-field-dto-schema.json
slug: factset-irn-configuration-create-custom-symbol-custom-field-dto
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateCustomSymbolCustomFieldDto\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type can be one of Text, SingleOption, MultiOptions, Numeric, Date, ExtendedText, ContactLookup\"\n    },\n    \"isHidden\": {\n      \"type\": \"boolean\"\n    },\n    \"isMandatory\": {\n      \"type\": \"boolean\"\n    },\n    \"isShownInInfobox\": {\n      \"type\": \"boolean\"\n    },\n    \"optionsConfig\": {\n      \"type\": \"array\"\n    },\n    \"customSymbolTypes\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-irn-configuration-create-custom-symbol-custom-field-dto-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: CreateCustomSymbolCustomFieldDto
---
