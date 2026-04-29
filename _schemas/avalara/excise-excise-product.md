---
description: ExciseProduct schema from Avalara API
layout: schema
name: ExciseProduct
properties_list:
- description: ''
  name: productCode
  type: string
- description: ''
  name: productName
  type: string
- description: ''
  name: productCategory
  type: string
- description: ''
  name: unitOfMeasure
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/excise-excise-product-schema.json
slug: excise-excise-product
source_filename: excise-excise-product-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/excise-excise-product-schema.json\",\n  \"title\": \"ExciseProduct\",\n  \"description\": \"ExciseProduct schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"productCode\": {\n      \"type\": \"string\"\n    },\n    \"productName\": {\n      \"type\": \"string\"\n    },\n    \"productCategory\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"MotorFuel\",\n        \"Diesel\",\n        \"Aviation\",\n        \"Alcohol\",\n        \"Tobacco\",\n        \"NaturalGas\",\n        \"Other\"\n      ]\n    },\n    \"unitOfMeasure\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/excise-excise-product-schema.json
tags:
- Taxes
title: ExciseProduct
---
