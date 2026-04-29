---
description: Describes subscription
layout: schema
name: SubscriptionContract
properties_list:
- description: Identifier of a subscription. Use this ID to control the subscription in future (e.g. update or delete).
  name: id
  type: string
- description: Specifies if the subscription is active
  name: isActive
  type: boolean
- description: ''
  name: billingType
  type: object
- description: Time (UTC) before which subscription must be activated (may be applicable to some non-active newly created subscriptions)
  name: activateBeforeUtc
  type: string
- description: Time (UTC) when subscription expires and will be removed. If not specified, subscription never expires.
  name: expiresOnUtc
  type: string
- description: Time (UTC) when subscription was created
  name: createdOnUtc
  type: string
- description: ''
  name: subject
  type: object
- description: ''
  name: subscriber
  type: object
- description: Additional messages
  name: notices
  type: array
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-subscription-contract-schema.json
slug: aerodatabox-subscription-contract
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-subscription-contract-schema.json\",\n  \"title\": \"SubscriptionContract\",\n  \"description\": \"Describes subscription\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of a subscription. \\r\\nUse this ID to control the subscription in future (e.g. update or delete).\",\n      \"format\": \"uuid\"\n    },\n    \"isActive\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies if the subscription is active\"\n    },\n    \"billingType\": {\n      \"$ref\": \"#/components/schemas/SubscriptionBillingType\"\n    },\n    \"activateBeforeUtc\": {\n      \"type\": \"string\",\n      \"description\": \"Time (UTC) before which subscription must be activated (may be applicable to \\r\\nsome non-active newly\
  \ created subscriptions)\",\n      \"format\": \"date-time\",\n      \"nullable\": true\n    },\n    \"expiresOnUtc\": {\n      \"type\": \"string\",\n      \"description\": \"Time (UTC) when subscription expires and will be removed.\\r\\n\\r\\nIf not specified, subscription never expires.\",\n      \"format\": \"date-time\",\n      \"nullable\": true\n    },\n    \"createdOnUtc\": {\n      \"type\": \"string\",\n      \"description\": \"Time (UTC) when subscription was created\",\n      \"format\": \"date-time\"\n    },\n    \"subject\": {\n      \"$ref\": \"#/components/schemas/SubscriptionSubjectContract\"\n    },\n    \"subscriber\": {\n      \"$ref\": \"#/components/schemas/SubscriberContract\"\n    },\n    \"notices\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Additional messages\",\n      \"nullable\": true\n    }\n  },\n  \"required\": [\n    \"createdOnUtc\",\n    \"id\",\n    \"isActive\",\n    \"subject\"\
  ,\n    \"subscriber\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-subscription-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: SubscriptionContract
---
