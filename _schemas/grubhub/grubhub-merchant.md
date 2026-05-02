---
description: A merchant on the Grubhub platform with store details, fulfillment settings, schedules, and operational status.
layout: schema
name: Grubhub Merchant
properties_list:
- description: The Grubhub internal merchant identifier.
  name: merchant_id
  type: string
- description: The partner's external merchant identifier.
  name: external_id
  type: string
- description: The merchant's display name.
  name: name
  type: string
- description: The current online/offline status of the merchant on Grubhub.
  name: status
  type: string
- description: The type of pause applied when merchant is offline. A soft pause is for the remainder of the business day; a hard pause is for multiple days.
  name: pause_type
  type:
  - string
  - 'null'
- description: ''
  name: address
  type: object
- description: The merchant's phone number.
  name: phone
  type: string
- description: The merchant's applicable tax rate as a decimal.
  name: tax_rate
  type: number
- description: Supported fulfillment types for this merchant.
  name: fulfillment_types
  type: array
- description: ''
  name: fulfillment_settings
  type: object
- description: Types of cuisine offered by the merchant.
  name: cuisine_types
  type: array
provider_name: grubhub
provider_slug: grubhub
schema_file: json-schema/grubhub-merchant-schema.json
slug: grubhub-merchant
source_filename: grubhub-merchant-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.grubhub.com/schemas/grubhub/merchant.json\",\n  \"title\": \"Grubhub Merchant\",\n  \"description\": \"A merchant on the Grubhub platform with store details, fulfillment settings, schedules, and operational status.\",\n  \"type\": \"object\",\n  \"required\": [\"merchant_id\", \"name\"],\n  \"properties\": {\n    \"merchant_id\": {\n      \"type\": \"string\",\n      \"description\": \"The Grubhub internal merchant identifier.\"\n    },\n    \"external_id\": {\n      \"type\": \"string\",\n      \"description\": \"The partner's external merchant identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The merchant's display name.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current online/offline status of the merchant on Grubhub.\",\n      \"enum\": [\"ONLINE\", \"OFFLINE\"]\n    },\n    \"pause_type\"\
  : {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The type of pause applied when merchant is offline. A soft pause is for the remainder of the business day; a hard pause is for multiple days.\",\n      \"enum\": [\"SOFT\", \"HARD\", null]\n    },\n    \"address\": {\n      \"$ref\": \"#/$defs/Address\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"The merchant's phone number.\"\n    },\n    \"tax_rate\": {\n      \"type\": \"number\",\n      \"description\": \"The merchant's applicable tax rate as a decimal.\",\n      \"minimum\": 0,\n      \"maximum\": 1\n    },\n    \"fulfillment_types\": {\n      \"type\": \"array\",\n      \"description\": \"Supported fulfillment types for this merchant.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"DELIVERY\", \"PICKUP\", \"CATERING\"]\n      }\n    },\n    \"fulfillment_settings\": {\n      \"$ref\": \"#/$defs/FulfillmentSettings\"\n    },\n    \"cuisine_types\"\
  : {\n      \"type\": \"array\",\n      \"description\": \"Types of cuisine offered by the merchant.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"Address\": {\n      \"type\": \"object\",\n      \"description\": \"A physical address for the merchant location.\",\n      \"properties\": {\n        \"street_address\": {\n          \"type\": \"string\",\n          \"description\": \"The street address line.\"\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"The city name.\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"The state abbreviation.\",\n          \"maxLength\": 2\n        },\n        \"zip\": {\n          \"type\": \"string\",\n          \"description\": \"The ZIP code.\",\n          \"pattern\": \"^\\\\d{5}(-\\\\d{4})?$\"\n        },\n        \"latitude\": {\n          \"type\": \"number\",\n          \"description\": \"The latitude\
  \ coordinate.\"\n        },\n        \"longitude\": {\n          \"type\": \"number\",\n          \"description\": \"The longitude coordinate.\"\n        }\n      }\n    },\n    \"FulfillmentSettings\": {\n      \"type\": \"object\",\n      \"description\": \"Fulfillment configuration for a merchant.\",\n      \"properties\": {\n        \"delivery_enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether delivery is enabled.\"\n        },\n        \"pickup_enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether pickup is enabled.\"\n        },\n        \"catering_enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether catering is enabled.\"\n        },\n        \"estimated_prep_time_minutes\": {\n          \"type\": \"integer\",\n          \"description\": \"Estimated preparation time in minutes.\",\n          \"minimum\": 0\n        },\n        \"delivery_radius_miles\": {\n          \"type\": \"number\"\
  ,\n          \"description\": \"The delivery radius in miles.\",\n          \"minimum\": 0\n        },\n        \"minimum_order_amount\": {\n          \"type\": \"number\",\n          \"description\": \"The minimum order amount for delivery.\",\n          \"minimum\": 0\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/json-schema/grubhub-merchant-schema.json
tags: []
title: Grubhub Merchant
---
