---
description: A tag applied to a monitored entity.
layout: schema
name: EntityTag
properties_list:
- description: The origin context of the tag. For example, CONTEXTLESS, ENVIRONMENT, AWS, KUBERNETES, etc.
  name: context
  type: string
- description: The key of the tag.
  name: key
  type: string
- description: The value of the tag, if applicable.
  name: value
  type: string
- description: The full string representation of the tag as displayed in the Dynatrace UI, e.g., [KUBERNETES]app:my-service.
  name: stringRepresentation
  type: string
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/entities-api-v2-entity-tag-schema.json
slug: entities-api-v2-entity-tag
source_filename: entities-api-v2-entity-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/entities-api-v2-entity-tag-schema.json\",\n  \"title\": \"EntityTag\",\n  \"description\": \"A tag applied to a monitored entity.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"context\": {\n      \"type\": \"string\",\n      \"description\": \"The origin context of the tag. For example, CONTEXTLESS, ENVIRONMENT, AWS, KUBERNETES, etc.\",\n      \"example\": \"example-value\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The key of the tag.\",\n      \"example\": \"example-value\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The value of the tag, if applicable.\",\n      \"nullable\": true,\n      \"example\": \"example-value\"\n    },\n    \"stringRepresentation\": {\n      \"type\": \"string\",\n      \"description\": \"The full string\
  \ representation of the tag as displayed in the Dynatrace UI, e.g., [KUBERNETES]app:my-service.\",\n      \"example\": \"example-value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/entities-api-v2-entity-tag-schema.json
tags:
- AI Operations
- Analytics
- APM
- Application Performance Monitoring
- Application Security
- Automation
- Cloud Monitoring
- Digital Experience Management
- Intelligence
- Observability
title: EntityTag
---
