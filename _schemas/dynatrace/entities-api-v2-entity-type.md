---
description: Defines an entity type including its display name, available properties, and supported relationship types.
layout: schema
name: EntityType
properties_list:
- description: The entity type identifier, e.g., SERVICE.
  name: type
  type: string
- description: The human-readable display name of the entity type.
  name: displayName
  type: string
- description: A description of what this entity type represents.
  name: description
  type: string
- description: The list of properties available for this entity type.
  name: properties
  type: array
- description: The relationship types where entities of this type are the source.
  name: fromRelationships
  type: array
- description: The relationship types where entities of this type are the target.
  name: toRelationships
  type: array
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/entities-api-v2-entity-type-schema.json
slug: entities-api-v2-entity-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/entities-api-v2-entity-type-schema.json\",\n  \"title\": \"EntityType\",\n  \"description\": \"Defines an entity type including its display name, available properties, and supported relationship types.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The entity type identifier, e.g., SERVICE.\",\n      \"example\": \"STANDARD\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable display name of the entity type.\",\n      \"example\": \"Production Service\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of what this entity type represents.\",\n      \"example\": \"Example description.\"\n    },\n    \"properties\": {\n      \"type\"\
  : \"array\",\n      \"description\": \"The list of properties available for this entity type.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/EntityTypeProperty\"\n      },\n      \"example\": [\n        {\n          \"id\": \"abc123\",\n          \"displayName\": \"Production Service\",\n          \"type\": \"STANDARD\"\n        }\n      ]\n    },\n    \"fromRelationships\": {\n      \"type\": \"array\",\n      \"description\": \"The relationship types where entities of this type are the source.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/EntityTypeRelationship\"\n      },\n      \"example\": [\n        {\n          \"id\": \"abc123\",\n          \"toTypes\": [\n            {}\n          ]\n        }\n      ]\n    },\n    \"toRelationships\": {\n      \"type\": \"array\",\n      \"description\": \"The relationship types where entities of this type are the target.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/EntityTypeRelationship\"\
  \n      },\n      \"example\": [\n        {\n          \"id\": \"abc123\",\n          \"toTypes\": [\n            {}\n          ]\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/entities-api-v2-entity-type-schema.json
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
title: EntityType
---
