---
description: AttributionRequest schema from Amplitude Attribution API
layout: schema
name: AttributionRequest
properties_list:
- description: The API key for the Amplitude project.
  name: api_key
  type: string
- description: ''
  name: event
  type: object
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/attribution-api-attribution-request-schema.json
slug: attribution-api-attribution-request
source_filename: attribution-api-attribution-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/attribution-api-attribution-request-schema.json\",\n  \"title\": \"AttributionRequest\",\n  \"description\": \"AttributionRequest schema from Amplitude Attribution API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"api_key\": {\n      \"type\": \"string\",\n      \"description\": \"The API key for the Amplitude project.\"\n    },\n    \"event\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"event_type\"\n      ],\n      \"properties\": {\n        \"user_id\": {\n          \"type\": \"string\",\n          \"description\": \"The user ID to attribute the campaign event to. Required unless device_id is present.\"\n        },\n        \"device_id\": {\n          \"type\": \"string\",\n          \"description\": \"The device ID. Required unless user_id is present.\"\n        },\n      \
  \  \"event_type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of attribution event, typically a campaign-related event such as install or re-engage.\"\n        },\n        \"platform\": {\n          \"type\": \"string\",\n          \"description\": \"The platform of the device, such as iOS or Android.\"\n        },\n        \"os_name\": {\n          \"type\": \"string\",\n          \"description\": \"The operating system name.\"\n        },\n        \"os_version\": {\n          \"type\": \"string\",\n          \"description\": \"The operating system version.\"\n        },\n        \"device_brand\": {\n          \"type\": \"string\",\n          \"description\": \"The brand of the device.\"\n        },\n        \"device_manufacturer\": {\n          \"type\": \"string\",\n          \"description\": \"The manufacturer of the device.\"\n        },\n        \"device_model\": {\n          \"type\": \"string\",\n          \"description\": \"The model of the device.\"\
  \n        },\n        \"carrier\": {\n          \"type\": \"string\",\n          \"description\": \"The carrier of the device.\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"description\": \"The country of the user.\"\n        },\n        \"region\": {\n          \"type\": \"string\",\n          \"description\": \"The region or state of the user.\"\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"The city of the user.\"\n        },\n        \"language\": {\n          \"type\": \"string\",\n          \"description\": \"The language setting of the user.\"\n        },\n        \"adid\": {\n          \"type\": \"string\",\n          \"description\": \"The Google Play Services advertising ID (Android).\"\n        },\n        \"idfa\": {\n          \"type\": \"string\",\n          \"description\": \"The Identifier for Advertiser (iOS).\"\n        },\n        \"idfv\": {\n          \"type\": \"string\",\n    \
  \      \"description\": \"The Identifier for Vendor (iOS).\"\n        },\n        \"user_properties\": {\n          \"type\": \"object\",\n          \"description\": \"User property operations to set alongside the attribution event. Typically used to set campaign-related properties like utm_source, utm_medium, utm_campaign, utm_term, and utm_content.\",\n          \"additionalProperties\": true\n        },\n        \"event_properties\": {\n          \"type\": \"object\",\n          \"description\": \"Additional properties associated with the attribution event such as campaign name, ad group, ad creative, and network.\",\n          \"additionalProperties\": true\n        },\n        \"time\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"The timestamp of the event in milliseconds since epoch.\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"api_key\",\n    \"event\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/attribution-api-attribution-request-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: AttributionRequest
---
