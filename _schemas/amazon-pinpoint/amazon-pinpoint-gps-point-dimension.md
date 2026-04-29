---
description: Specifies GPS-based criteria for including or excluding endpoints from a segment.
layout: schema
name: GPSPointDimension
properties_list:
- description: ''
  name: Coordinates
  type: object
- description: ''
  name: RangeInKilometers
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-gps-point-dimension-schema.json
slug: amazon-pinpoint-gps-point-dimension
source_filename: amazon-pinpoint-gps-point-dimension-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-gps-point-dimension-schema.json\",\n  \"title\": \"GPSPointDimension\",\n  \"description\": \"Specifies GPS-based criteria for including or excluding endpoints from a segment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Coordinates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GPSCoordinates\"\n        },\n        {\n          \"description\": \"The GPS coordinates to measure distance from.\"\n        }\n      ]\n    },\n    \"RangeInKilometers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"description\": \"The range, in kilometers, from the GPS coordinates.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Coordinates\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-gps-point-dimension-schema.json
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
title: GPSPointDimension
---
