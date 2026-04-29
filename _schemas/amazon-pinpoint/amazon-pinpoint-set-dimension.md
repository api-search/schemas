---
description: Specifies the dimension type and values for a segment dimension.
layout: schema
name: SetDimension
properties_list:
- description: ''
  name: DimensionType
  type: object
- description: ''
  name: Values
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-set-dimension-schema.json
slug: amazon-pinpoint-set-dimension
source_filename: amazon-pinpoint-set-dimension-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-set-dimension-schema.json\",\n  \"title\": \"SetDimension\",\n  \"description\": \"Specifies the dimension type and values for a segment dimension.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DimensionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DimensionType\"\n        },\n        {\n          \"description\": \"The type of segment dimension to use. Valid values are: INCLUSIVE, endpoints that match the criteria are included in the segment; and, EXCLUSIVE, endpoints that match the criteria are excluded from the segment.\"\n        }\n      ]\n    },\n    \"Values\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOf__string\"\n        },\n        {\n          \"description\": \"The criteria values to use\
  \ for the segment dimension. Depending on the value of the DimensionType property, endpoints are included or excluded from the segment if their values match the criteria values.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Values\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-set-dimension-schema.json
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
title: SetDimension
---
