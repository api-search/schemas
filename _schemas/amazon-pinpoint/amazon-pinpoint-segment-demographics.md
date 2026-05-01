---
description: Specifies demographic-based dimension settings for including or excluding endpoints from a segment. These settings derive from characteristics of endpoint devices, such as platform, make, and model.
layout: schema
name: SegmentDemographics
properties_list:
- description: ''
  name: AppVersion
  type: object
- description: ''
  name: Channel
  type: object
- description: ''
  name: DeviceType
  type: object
- description: ''
  name: Make
  type: object
- description: ''
  name: Model
  type: object
- description: ''
  name: Platform
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-segment-demographics-schema.json
slug: amazon-pinpoint-segment-demographics
source_filename: amazon-pinpoint-segment-demographics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-segment-demographics-schema.json\",\n  \"title\": \"SegmentDemographics\",\n  \"description\": \"Specifies demographic-based dimension settings for including or excluding endpoints from a segment. These settings derive from characteristics of endpoint devices, such as platform, make, and model.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AppVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SetDimension\"\n        },\n        {\n          \"description\": \"The app version criteria for the segment.\"\n        }\n      ]\n    },\n    \"Channel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SetDimension\"\n        },\n        {\n          \"description\": \"The channel criteria for the segment.\"\n        }\n\
  \      ]\n    },\n    \"DeviceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SetDimension\"\n        },\n        {\n          \"description\": \"The device type criteria for the segment.\"\n        }\n      ]\n    },\n    \"Make\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SetDimension\"\n        },\n        {\n          \"description\": \"The device make criteria for the segment.\"\n        }\n      ]\n    },\n    \"Model\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SetDimension\"\n        },\n        {\n          \"description\": \"The device model criteria for the segment.\"\n        }\n      ]\n    },\n    \"Platform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SetDimension\"\n        },\n        {\n          \"description\": \"The device platform criteria for the segment.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-segment-demographics-schema.json
tags:
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
title: SegmentDemographics
---
