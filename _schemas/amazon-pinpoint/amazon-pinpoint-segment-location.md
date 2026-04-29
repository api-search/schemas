---
description: Specifies geographical dimension settings for a segment.
layout: schema
name: SegmentLocation
properties_list:
- description: ''
  name: Country
  type: object
- description: ''
  name: GPSPoint
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-segment-location-schema.json
slug: amazon-pinpoint-segment-location
source_filename: amazon-pinpoint-segment-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-segment-location-schema.json\",\n  \"title\": \"SegmentLocation\",\n  \"description\": \"Specifies geographical dimension settings for a segment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Country\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SetDimension\"\n        },\n        {\n          \"description\": \"The country or region code, in ISO 3166-1 alpha-2 format, for the segment.\"\n        }\n      ]\n    },\n    \"GPSPoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GPSPointDimension\"\n        },\n        {\n          \"description\": \"The GPS location and range for the segment.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-segment-location-schema.json
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
title: SegmentLocation
---
