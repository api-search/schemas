---
description: Request to configure phone number features
layout: schema
name: FeatureOrderRequest
properties_list:
- description: ''
  name: callingNameDisplay
  type: object
- description: ''
  name: directoryListing
  type: object
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/phone-numbers-feature-order-request-schema.json
slug: phone-numbers-feature-order-request
source_filename: phone-numbers-feature-order-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-feature-order-request-schema.json\",\n  \"title\": \"FeatureOrderRequest\",\n  \"description\": \"Request to configure phone number features\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"callingNameDisplay\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether CNAM display is enabled\"\n        },\n        \"callingName\": {\n          \"type\": \"string\",\n          \"maxLength\": 15,\n          \"description\": \"The caller name to display (max 15 characters)\"\n        }\n      }\n    },\n    \"directoryListing\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"listed\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the number is listed\
  \ in the directory\"\n        },\n        \"listingType\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"LISTED\",\n            \"NON_LISTED\",\n            \"NON_PUBLISHED\"\n          ],\n          \"description\": \"The type of directory listing\"\n        },\n        \"listingName\": {\n          \"type\": \"string\",\n          \"description\": \"The name for the directory listing\"\n        },\n        \"listAddress\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to list the address in the directory\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-feature-order-request-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: FeatureOrderRequest
---
