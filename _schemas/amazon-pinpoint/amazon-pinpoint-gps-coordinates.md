---
description: Specifies the GPS coordinates of a location.
layout: schema
name: GPSCoordinates
properties_list:
- description: ''
  name: Latitude
  type: object
- description: ''
  name: Longitude
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-gps-coordinates-schema.json
slug: amazon-pinpoint-gps-coordinates
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-gps-coordinates-schema.json\",\n  \"title\": \"GPSCoordinates\",\n  \"description\": \"Specifies the GPS coordinates of a location.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Latitude\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"description\": \"The latitude coordinate of the location.\"\n        }\n      ]\n    },\n    \"Longitude\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"description\": \"The longitude coordinate of the location.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Latitude\",\n    \"Longitude\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-gps-coordinates-schema.json
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
title: GPSCoordinates
---
