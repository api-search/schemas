---
description: Internal configuration data returned with the promo response.
layout: schema
name: PromoConfig
properties_list:
- description: Indicates whether prequalification is enabled for this merchant.
  name: promo_prequal_enabled
  type: boolean
- description: The merchant's display name.
  name: merchant_name
  type: string
- description: Affirm Resource Identifier for the merchant.
  name: merchant_ari
  type: string
- description: Affirm Resource Identifier for the current user session.
  name: user_ari
  type: string
- description: Indicates whether toast notifications are enabled for this integration.
  name: toast_enabled
  type: boolean
- description: List of enabled Affirm integration features for this merchant.
  name: enabled_integrations
  type: array
- description: Image asset URLs for use in the promotional modal.
  name: images
  type: object
provider_name: affirm
provider_slug: affirm
schema_file: json-schema/promos-promo-config-schema.json
slug: promos-promo-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/promos-promo-config-schema.json\",\n  \"title\": \"PromoConfig\",\n  \"description\": \"Internal configuration data returned with the promo response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"promo_prequal_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether prequalification is enabled for this merchant.\",\n      \"example\": true\n    },\n    \"merchant_name\": {\n      \"type\": \"string\",\n      \"description\": \"The merchant's display name.\",\n      \"example\": \"Example Merchant\"\n    },\n    \"merchant_ari\": {\n      \"type\": \"string\",\n      \"description\": \"Affirm Resource Identifier for the merchant.\",\n      \"example\": \"example_value\"\n    },\n    \"user_ari\": {\n      \"type\": \"string\",\n      \"description\": \"Affirm Resource Identifier\
  \ for the current user session.\",\n      \"example\": \"example_value\"\n    },\n    \"toast_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether toast notifications are enabled for this integration.\",\n      \"example\": true\n    },\n    \"enabled_integrations\": {\n      \"type\": \"array\",\n      \"description\": \"List of enabled Affirm integration features for this merchant.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"example_value\"\n      ]\n    },\n    \"images\": {\n      \"type\": \"object\",\n      \"description\": \"Image asset URLs for use in the promotional modal.\",\n      \"properties\": {\n        \"hero\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Standard resolution hero image URL.\"\n        },\n        \"hero2x\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"High resolution\
  \ (2x) hero image URL.\"\n        },\n        \"logo\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Standard resolution Affirm logo URL.\"\n        },\n        \"logo2x\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"High resolution (2x) Affirm logo URL.\"\n        }\n      },\n      \"example\": {\n        \"hero\": \"https://example.com\",\n        \"hero2x\": \"https://example.com\",\n        \"logo\": \"https://example.com\",\n        \"logo2x\": \"https://example.com\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/promos-promo-config-schema.json
tags: []
title: PromoConfig
---
