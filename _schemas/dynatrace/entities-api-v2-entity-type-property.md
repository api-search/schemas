---
description: Describes a single property of an entity type.
layout: schema
name: EntityTypeProperty
properties_list:
- description: The property key identifier.
  name: id
  type: string
- description: The human-readable display name of the property.
  name: displayName
  type: string
- description: The data type of the property value.
  name: type
  type: string
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/entities-api-v2-entity-type-property-schema.json
slug: entities-api-v2-entity-type-property
source_filename: entities-api-v2-entity-type-property-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/entities-api-v2-entity-type-property-schema.json\",\n  \"title\": \"EntityTypeProperty\",\n  \"description\": \"Describes a single property of an entity type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The property key identifier.\",\n      \"example\": \"abc123\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable display name of the property.\",\n      \"example\": \"Production Service\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The data type of the property value.\",\n      \"example\": \"STANDARD\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/entities-api-v2-entity-type-property-schema.json
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
title: EntityTypeProperty
---
