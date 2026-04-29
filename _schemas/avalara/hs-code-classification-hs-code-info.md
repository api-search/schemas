---
description: HSCodeInfo schema from Avalara API
layout: schema
name: HSCodeInfo
properties_list:
- description: ''
  name: hsCode
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: level
  type: string
- description: ''
  name: parentCode
  type: string
- description: ''
  name: dutyRate
  type: string
- description: ''
  name: unitOfMeasure
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/hs-code-classification-hs-code-info-schema.json
slug: hs-code-classification-hs-code-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/hs-code-classification-hs-code-info-schema.json\",\n  \"title\": \"HSCodeInfo\",\n  \"description\": \"HSCodeInfo schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"hsCode\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"level\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Section\",\n        \"Chapter\",\n        \"Heading\",\n        \"Subheading\",\n        \"TariffLine\"\n      ]\n    },\n    \"parentCode\": {\n      \"type\": \"string\"\n    },\n    \"dutyRate\": {\n      \"type\": \"string\"\n    },\n    \"unitOfMeasure\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/hs-code-classification-hs-code-info-schema.json
tags:
- Taxes
title: HSCodeInfo
---
