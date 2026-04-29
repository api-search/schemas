---
description: Provides information about all the endpoints that are associated with a user ID.
layout: schema
name: EndpointsResponse
properties_list:
- description: ''
  name: Item
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-endpoints-response-schema.json
slug: amazon-pinpoint-endpoints-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-endpoints-response-schema.json\",\n  \"title\": \"EndpointsResponse\",\n  \"description\": \"Provides information about all the endpoints that are associated with a user ID.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Item\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfEndpointResponse\"\n        },\n        {\n          \"description\": \"An array of responses, one for each endpoint that's associated with the user ID.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Item\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-endpoints-response-schema.json
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
title: EndpointsResponse
---
