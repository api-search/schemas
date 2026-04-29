---
description: A lightweight reference to a monitored entity.
layout: schema
name: EntityStub
properties_list:
- description: The unique identifier of the entity, e.g., SERVICE-1234567890ABCDEF.
  name: entityId
  type: string
- description: The display name of the entity.
  name: name
  type: string
- description: The type of the entity, e.g., SERVICE, HOST, PROCESS_GROUP, APPLICATION.
  name: type
  type: string
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/dynatrace-problems-v2-entity-stub-schema.json
slug: dynatrace-problems-v2-entity-stub
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A lightweight reference to a monitored entity.\",\n  \"properties\": {\n    \"entityId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the entity, e.g., SERVICE-1234567890ABCDEF.\",\n      \"example\": \"abc123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the entity.\",\n      \"example\": \"Production Service\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the entity, e.g., SERVICE, HOST, PROCESS_GROUP, APPLICATION.\",\n      \"example\": \"STANDARD\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EntityStub\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-problems-v2-entity-stub-schema.json
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
title: EntityStub
---
