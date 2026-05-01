---
description: Specifies data for one or more attributes that describe the user who's associated with an endpoint.
layout: schema
name: EndpointUser
properties_list:
- description: ''
  name: UserAttributes
  type: object
- description: ''
  name: UserId
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-endpoint-user-schema.json
slug: amazon-pinpoint-endpoint-user
source_filename: amazon-pinpoint-endpoint-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-endpoint-user-schema.json\",\n  \"title\": \"EndpointUser\",\n  \"description\": \"Specifies data for one or more attributes that describe the user who's associated with an endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfListOf__string\"\n        },\n        {\n          \"description\": \"<p>One or more custom attributes that describe the user by associating a name with an array of values. For example, the value of an attribute named Interests might be: [\\\"Science\\\", \\\"Music\\\", \\\"Travel\\\"]. You can use these attributes as filter criteria when you create segments. Attribute names are case sensitive.</p> <p>An attribute name can contain up to 50 characters. An\
  \ attribute value can contain up to 100 characters. When you define the name of a custom attribute, avoid using the following characters: number sign (#), colon (:), question mark (?), backslash (\\\\), and slash (/). The Amazon Pinpoint console can't display attribute names that contain these characters. This restriction doesn't apply to attribute values.</p>\"\n        }\n      ]\n    },\n    \"UserId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the user.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-endpoint-user-schema.json
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
title: EndpointUser
---
