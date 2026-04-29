---
description: Request body for looking up an entity by name and type.
layout: schema
name: EntityLookupRequest
properties_list:
- description: The display name of the entity to look up.
  name: name
  type: string
- description: The entity type to search within, e.g., SERVICE, HOST.
  name: type
  type: string
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/entities-api-v2-entity-lookup-request-schema.json
slug: entities-api-v2-entity-lookup-request
source_filename: entities-api-v2-entity-lookup-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/entities-api-v2-entity-lookup-request-schema.json\",\n  \"title\": \"EntityLookupRequest\",\n  \"description\": \"Request body for looking up an entity by name and type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the entity to look up.\",\n      \"example\": \"Production Service\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The entity type to search within, e.g., SERVICE, HOST.\",\n      \"example\": \"STANDARD\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/entities-api-v2-entity-lookup-request-schema.json
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
title: EntityLookupRequest
---
