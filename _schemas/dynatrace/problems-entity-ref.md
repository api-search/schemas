---
description: A reference to a monitored entity in problem details.
layout: schema
name: EntityRef
properties_list:
- description: The unique Dynatrace entity ID.
  name: entityId
  type: string
- description: The display name of the entity.
  name: name
  type: string
- description: The entity type, e.g., SERVICE, HOST, PROCESS_GROUP.
  name: type
  type: string
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/problems-entity-ref-schema.json
slug: problems-entity-ref
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/problems-entity-ref-schema.json\",\n  \"title\": \"EntityRef\",\n  \"description\": \"A reference to a monitored entity in problem details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entityId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique Dynatrace entity ID.\",\n      \"example\": \"SERVICE-ABCDEF1234567890\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the entity.\",\n      \"example\": \"payment-service\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The entity type, e.g., SERVICE, HOST, PROCESS_GROUP.\",\n      \"example\": \"SERVICE\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/problems-entity-ref-schema.json
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
title: EntityRef
---
