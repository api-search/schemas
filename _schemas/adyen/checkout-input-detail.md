---
description: InputDetail schema from Adyen API
layout: schema
name: InputDetail
properties_list:
- description: Configuration parameters for the required input.
  name: configuration
  type: object
- description: Input details can also be provided recursively.
  name: details
  type: array
- description: Input details can also be provided recursively (deprecated).
  name: inputDetails
  type: array
- description: In case of a select, the URL from which to query the items.
  name: itemSearchUrl
  type: string
- description: In case of a select, the items to choose from.
  name: items
  type: array
- description: The value to provide in the result.
  name: key
  type: string
- description: True if this input value is optional.
  name: optional
  type: boolean
- description: The type of the required input.
  name: type
  type: string
- description: The value can be pre-filled, if available.
  name: value
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-input-detail-schema.json
slug: checkout-input-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-input-detail-schema.json\",\n  \"title\": \"InputDetail\",\n  \"description\": \"InputDetail schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configuration\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Configuration parameters for the required input.\",\n      \"type\": \"object\"\n    },\n    \"details\": {\n      \"description\": \"Input details can also be provided recursively.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SubInputDetail\"\n      },\n      \"type\": \"array\"\n    },\n    \"inputDetails\": {\n      \"deprecated\": true,\n      \"description\": \"Input details can also be provided recursively (deprecated).\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SubInputDetail\"\
  \n      },\n      \"type\": \"array\"\n    },\n    \"itemSearchUrl\": {\n      \"description\": \"In case of a select, the URL from which to query the items.\",\n      \"type\": \"string\"\n    },\n    \"items\": {\n      \"description\": \"In case of a select, the items to choose from.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Item\"\n      },\n      \"type\": \"array\"\n    },\n    \"key\": {\n      \"description\": \"The value to provide in the result.\",\n      \"type\": \"string\"\n    },\n    \"optional\": {\n      \"description\": \"True if this input value is optional.\",\n      \"type\": \"boolean\"\n    },\n    \"type\": {\n      \"description\": \"The type of the required input.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"The value can be pre-filled, if available.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-input-detail-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: InputDetail
---
