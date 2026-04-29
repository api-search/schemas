---
description: A paginated collection of entity type definitions.
layout: schema
name: EntityTypeCollection
properties_list:
- description: Cursor for the next page of results.
  name: nextPageKey
  type: string
- description: The total number of entity types.
  name: totalCount
  type: integer
- description: The list of entity types on this page.
  name: types
  type: array
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/entities-api-v2-entity-type-collection-schema.json
slug: entities-api-v2-entity-type-collection
source_filename: entities-api-v2-entity-type-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/entities-api-v2-entity-type-collection-schema.json\",\n  \"title\": \"EntityTypeCollection\",\n  \"description\": \"A paginated collection of entity type definitions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextPageKey\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor for the next page of results.\",\n      \"nullable\": true,\n      \"example\": \"example-value\"\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The total number of entity types.\",\n      \"example\": 500\n    },\n    \"types\": {\n      \"type\": \"array\",\n      \"description\": \"The list of entity types on this page.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/EntityType\"\n      },\n      \"example\": [\n        {\n\
  \          \"type\": \"STANDARD\",\n          \"displayName\": \"Production Service\",\n          \"description\": \"Example description.\",\n          \"properties\": [\n            {\n              \"id\": \"abc123\",\n              \"displayName\": \"Production Service\",\n              \"type\": \"STANDARD\"\n            }\n          ],\n          \"fromRelationships\": [\n            {\n              \"id\": \"abc123\",\n              \"toTypes\": [\n                {}\n              ]\n            }\n          ],\n          \"toRelationships\": [\n            {\n              \"id\": \"abc123\",\n              \"toTypes\": [\n                {}\n              ]\n            }\n          ]\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/entities-api-v2-entity-type-collection-schema.json
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
title: EntityTypeCollection
---
