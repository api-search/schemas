---
description: Detail data for a resource sync event.
layout: schema
name: ResourceSyncEvent
properties_list:
- description: ''
  name: event
  type: object
- description: ''
  name: externalId
  type: object
- description: ''
  name: time
  type: object
- description: ''
  name: type
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-resource-sync-event-schema.json
slug: amazon-proton-resource-sync-event
source_filename: amazon-proton-resource-sync-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-resource-sync-event-schema.json\",\n  \"title\": \"ResourceSyncEvent\",\n  \"description\": \"Detail data for a resource sync event.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"event\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A resource sync event.\"\n        }\n      ]\n    },\n    \"externalId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The external ID for the event.\"\n        }\n      ]\n    },\n    \"time\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the event occurred.\"\
  \n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The type of event.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"event\",\n    \"time\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-resource-sync-event-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ResourceSyncEvent
---
