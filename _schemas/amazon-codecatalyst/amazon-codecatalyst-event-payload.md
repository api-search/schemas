---
description: Information about the payload of an event recording Amazon CodeCatalyst activity.
layout: schema
name: EventPayload
properties_list:
- description: ''
  name: contentType
  type: object
- description: ''
  name: data
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-event-payload-schema.json
slug: amazon-codecatalyst-event-payload
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-event-payload-schema.json\",\n  \"title\": \"EventPayload\",\n  \"description\": \"Information about the payload of an event recording Amazon CodeCatalyst activity.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contentType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The type of content in the event payload.\"\n        }\n      ]\n    },\n    \"data\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The data included in the event payload.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-event-payload-schema.json
tags:
- Amazon
- AWS
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: EventPayload
---
