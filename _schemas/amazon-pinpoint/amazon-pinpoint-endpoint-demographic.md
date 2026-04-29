---
description: Specifies demographic information about an endpoint, such as the applicable time zone and platform.
layout: schema
name: EndpointDemographic
properties_list:
- description: ''
  name: AppVersion
  type: object
- description: ''
  name: Locale
  type: object
- description: ''
  name: Make
  type: object
- description: ''
  name: Model
  type: object
- description: ''
  name: ModelVersion
  type: object
- description: ''
  name: Platform
  type: object
- description: ''
  name: PlatformVersion
  type: object
- description: ''
  name: Timezone
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-endpoint-demographic-schema.json
slug: amazon-pinpoint-endpoint-demographic
source_filename: amazon-pinpoint-endpoint-demographic-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-endpoint-demographic-schema.json\",\n  \"title\": \"EndpointDemographic\",\n  \"description\": \"Specifies demographic information about an endpoint, such as the applicable time zone and platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AppVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The version of the app that's associated with the endpoint.\"\n        }\n      ]\n    },\n    \"Locale\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The locale of the endpoint, in the following format: the ISO 639-1 alpha-2 code, followed by an underscore (_), followed by an ISO 3166-1 alpha-2\
  \ value.\"\n        }\n      ]\n    },\n    \"Make\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The manufacturer of the endpoint device, such as apple or samsung.\"\n        }\n      ]\n    },\n    \"Model\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The model name or number of the endpoint device, such as iPhone or SM-G900F.\"\n        }\n      ]\n    },\n    \"ModelVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The model version of the endpoint device.\"\n        }\n      ]\n    },\n    \"Platform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The platform of the endpoint device, such as ios.\"\
  \n        }\n      ]\n    },\n    \"PlatformVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The platform version of the endpoint device.\"\n        }\n      ]\n    },\n    \"Timezone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The time zone of the endpoint, specified as a tz database name value, such as America/Los_Angeles.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-endpoint-demographic-schema.json
tags:
- AWS
- Campaigns
- Communications
- Email
- Marketing
- Messaging
- Push Notifications
- SMS
- Voice
- Customer Engagement
- Segmentation
- Journeys
- Analytics
title: EndpointDemographic
---
