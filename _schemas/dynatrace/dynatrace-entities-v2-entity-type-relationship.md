---
description: Describes a relationship type for an entity type.
layout: schema
name: EntityTypeRelationship
properties_list:
- description: The relationship type identifier, e.g., runsOn.
  name: id
  type: string
- description: The entity types that can participate in this relationship.
  name: toTypes
  type: array
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/dynatrace-entities-v2-entity-type-relationship-schema.json
slug: dynatrace-entities-v2-entity-type-relationship
source_filename: dynatrace-entities-v2-entity-type-relationship-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Describes a relationship type for an entity type.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The relationship type identifier, e.g., runsOn.\",\n      \"example\": \"abc123\"\n    },\n    \"toTypes\": {\n      \"type\": \"array\",\n      \"description\": \"The entity types that can participate in this relationship.\",\n      \"example\": [\n        \"STANDARD\"\n      ],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EntityTypeRelationship\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-entities-v2-entity-type-relationship-schema.json
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
title: EntityTypeRelationship
---
