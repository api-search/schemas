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
schema_file: json-schema/dynatrace-entities-v2-entity-type-schema.json
slug: dynatrace-entities-v2-entity-type
source_filename: dynatrace-entities-v2-entity-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Defines an entity type including its display name, available properties, and supported relationship types.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The entity type identifier, e.g., SERVICE.\",\n      \"example\": \"STANDARD\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable display name of the entity type.\",\n      \"example\": \"Production Service\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of what this entity type represents.\",\n      \"example\": \"Example description.\"\n    },\n    \"properties\": {\n      \"type\": \"array\",\n      \"description\": \"The list of properties available for this entity type.\",\n      \"example\": [\n        {\n          \"id\": \"abc123\",\n          \"displayName\": \"Production Service\",\n          \"type\": \"STANDARD\"\
  \n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Describes a single property of an entity type.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The property key identifier.\",\n            \"example\": \"abc123\"\n          },\n          \"displayName\": {\n            \"type\": \"string\",\n            \"description\": \"The human-readable display name of the property.\",\n            \"example\": \"Production Service\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"The data type of the property value.\",\n            \"example\": \"STANDARD\"\n          }\n        }\n      }\n    },\n    \"fromRelationships\": {\n      \"type\": \"array\",\n      \"description\": \"The relationship types where entities of this type are the source.\",\n      \"example\": [\n        {\n          \"id\": \"abc123\",\n         \
  \ \"toTypes\": [\n            {}\n          ]\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Describes a relationship type for an entity type.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The relationship type identifier, e.g., runsOn.\",\n            \"example\": \"abc123\"\n          },\n          \"toTypes\": {\n            \"type\": \"array\",\n            \"description\": \"The entity types that can participate in this relationship.\",\n            \"example\": [\n              \"STANDARD\"\n            ],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"toRelationships\": {\n      \"type\": \"array\",\n      \"description\": \"The relationship types where entities of this type are the target.\",\n      \"example\": [\n        {\n          \"id\": \"abc123\",\n          \"toTypes\"\
  : [\n            {}\n          ]\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Describes a relationship type for an entity type.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The relationship type identifier, e.g., runsOn.\",\n            \"example\": \"abc123\"\n          },\n          \"toTypes\": {\n            \"type\": \"array\",\n            \"description\": \"The entity types that can participate in this relationship.\",\n            \"example\": [\n              \"STANDARD\"\n            ],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EntityType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-entities-v2-entity-type-schema.json
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
