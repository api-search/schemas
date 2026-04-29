---
description: Specifies a batch of endpoints to create or update and the settings and attributes to set or change for each endpoint.
layout: schema
name: EndpointBatchRequest
properties_list:
- description: ''
  name: Item
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-endpoint-batch-request-schema.json
slug: amazon-pinpoint-endpoint-batch-request
source_filename: amazon-pinpoint-endpoint-batch-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-endpoint-batch-request-schema.json\",\n  \"title\": \"EndpointBatchRequest\",\n  \"description\": \"Specifies a batch of endpoints to create or update and the settings and attributes to set or change for each endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Item\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfEndpointBatchItem\"\n        },\n        {\n          \"description\": \"An array that defines the endpoints to create or update and, for each endpoint, the property values to set or change. An array can contain a maximum of 100 items.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Item\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-endpoint-batch-request-schema.json
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
title: EndpointBatchRequest
---
