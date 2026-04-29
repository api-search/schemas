---
description: MultiDocumentLineItemModel schema from Avalara API
layout: schema
name: MultiDocumentLineItemModel
properties_list:
- description: ''
  name: companyCode
  type: string
- description: ''
  name: reportingLocationCode
  type: string
- description: ''
  name: number
  type: string
- description: ''
  name: quantity
  type: number
- description: ''
  name: amount
  type: number
- description: ''
  name: taxCode
  type: string
- description: ''
  name: addresses
  type: object
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-multi-document-line-item-model-schema.json
slug: avatax-rest-multi-document-line-item-model
source_filename: avatax-rest-multi-document-line-item-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-multi-document-line-item-model-schema.json\",\n  \"title\": \"MultiDocumentLineItemModel\",\n  \"description\": \"MultiDocumentLineItemModel schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"companyCode\": {\n      \"type\": \"string\"\n    },\n    \"reportingLocationCode\": {\n      \"type\": \"string\"\n    },\n    \"number\": {\n      \"type\": \"string\"\n    },\n    \"quantity\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"taxCode\": {\n      \"type\": \"string\"\n    },\n    \"addresses\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"shipFrom\": {\n          \"$ref\": \"#/components/schemas/AddressInfo\"\n        },\n       \
  \ \"shipTo\": {\n          \"$ref\": \"#/components/schemas/AddressInfo\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-multi-document-line-item-model-schema.json
tags:
- Taxes
title: MultiDocumentLineItemModel
---
