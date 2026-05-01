---
description: Specifies one or more attributes to remove from all the endpoints that are associated with an application.
layout: schema
name: UpdateAttributesRequest
properties_list:
- description: ''
  name: Blacklist
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-update-attributes-request-schema.json
slug: amazon-pinpoint-update-attributes-request
source_filename: amazon-pinpoint-update-attributes-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-update-attributes-request-schema.json\",\n  \"title\": \"UpdateAttributesRequest\",\n  \"description\": \"Specifies one or more attributes to remove from all the endpoints that are associated with an application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Blacklist\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOf__string\"\n        },\n        {\n          \"description\": \"An array of the attributes to remove from all the endpoints that are associated with the application. The array can specify the complete, exact name of each attribute to remove or it can specify a glob pattern that an attribute name must match in order for the attribute to be removed.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-update-attributes-request-schema.json
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
title: UpdateAttributesRequest
---
