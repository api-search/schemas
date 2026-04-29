---
description: Provides the status code and message that result from processing data for an endpoint.
layout: schema
name: EndpointItemResponse
properties_list:
- description: ''
  name: Message
  type: object
- description: ''
  name: StatusCode
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-endpoint-item-response-schema.json
slug: amazon-pinpoint-endpoint-item-response
source_filename: amazon-pinpoint-endpoint-item-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-endpoint-item-response-schema.json\",\n  \"title\": \"EndpointItemResponse\",\n  \"description\": \"Provides the status code and message that result from processing data for an endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The custom message that's returned in the response as a result of processing the endpoint data.\"\n        }\n      ]\n    },\n    \"StatusCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The status code that's returned in the response as a result of processing the endpoint data.\"\n        }\n     \
  \ ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-endpoint-item-response-schema.json
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
title: EndpointItemResponse
---
