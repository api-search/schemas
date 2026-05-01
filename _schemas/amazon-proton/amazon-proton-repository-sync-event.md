---
description: Repository sync event detail data for a sync attempt.
layout: schema
name: RepositorySyncEvent
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
schema_file: json-schema/amazon-proton-repository-sync-event-schema.json
slug: amazon-proton-repository-sync-event
source_filename: amazon-proton-repository-sync-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-repository-sync-event-schema.json\",\n  \"title\": \"RepositorySyncEvent\",\n  \"description\": \"Repository sync event detail data for a sync attempt.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"event\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Event detail for a repository sync attempt.\"\n        }\n      ]\n    },\n    \"externalId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The external ID of the sync event.\"\n        }\n      ]\n    },\n    \"time\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\"\
  : \"The time that the sync event occurred.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The type of event.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"event\",\n    \"time\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-repository-sync-event-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: RepositorySyncEvent
---
