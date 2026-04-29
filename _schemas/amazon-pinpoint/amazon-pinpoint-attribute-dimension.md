---
description: Specifies attribute-based criteria for including or excluding endpoints from a segment.
layout: schema
name: AttributeDimension
properties_list:
- description: ''
  name: AttributeType
  type: object
- description: ''
  name: Values
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-attribute-dimension-schema.json
slug: amazon-pinpoint-attribute-dimension
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-attribute-dimension-schema.json\",\n  \"title\": \"AttributeDimension\",\n  \"description\": \"Specifies attribute-based criteria for including or excluding endpoints from a segment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AttributeType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeType\"\n        },\n        {\n          \"description\": \"The type of segment dimension to use. Valid values are: <ul><li>INCLUSIVE - endpoints that have attributes matching the values are included in the segment.</li><li>EXCLUSIVE - endpoints that have attributes matching the values are excluded in the segment.</li><li>CONTAINS - endpoints that have attributes' substrings match the values are included in the segment.</li><li>BEFORE - endpoints with\
  \ attributes read as ISO_INSTANT datetimes before the value are included in the segment.</li><li>AFTER - endpoints with attributes read as ISO_INSTANT datetimes after the value are included in the segment.</li><li>ON - endpoints with attributes read as ISO_INSTANT dates on the value are included in the segment. Time is ignored in this comparison.</li><li>BETWEEN - endpoints with attributes read as ISO_INSTANT datetimes between the values are included in the segment.</li>\"\n        }\n      ]\n    },\n    \"Values\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOf__string\"\n        },\n        {\n          \"description\": \"The criteria values to use for the segment dimension. Depending on the value of the AttributeType property, endpoints are included or excluded from the segment if their attribute values match the criteria values.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Values\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-attribute-dimension-schema.json
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
title: AttributeDimension
---
