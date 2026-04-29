---
description: A paginated collection of monitored entities.
layout: schema
name: EntityCollection
properties_list:
- description: Cursor for the next page of results. Null if no more pages.
  name: nextPageKey
  type: string
- description: The total number of entities matching the query.
  name: totalCount
  type: integer
- description: The number of results returned on this page.
  name: pageSize
  type: integer
- description: The list of entities on this page.
  name: entities
  type: array
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/entities-api-v2-entity-collection-schema.json
slug: entities-api-v2-entity-collection
source_filename: entities-api-v2-entity-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/entities-api-v2-entity-collection-schema.json\",\n  \"title\": \"EntityCollection\",\n  \"description\": \"A paginated collection of monitored entities.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextPageKey\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor for the next page of results. Null if no more pages.\",\n      \"nullable\": true,\n      \"example\": \"example-value\"\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The total number of entities matching the query.\",\n      \"example\": 500\n    },\n    \"pageSize\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of results returned on this page.\",\n      \"example\": 500\n    },\n    \"entities\": {\n      \"type\": \"array\",\n \
  \     \"description\": \"The list of entities on this page.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Entity\"\n      },\n      \"example\": [\n        {\n          \"entityId\": \"abc123\",\n          \"displayName\": \"Production Service\",\n          \"type\": \"STANDARD\",\n          \"firstSeenTms\": 500,\n          \"lastSeenTms\": 500,\n          \"properties\": {},\n          \"tags\": [\n            {\n              \"context\": \"example-value\",\n              \"key\": \"example-value\",\n              \"value\": \"example-value\",\n              \"stringRepresentation\": \"example-value\"\n            }\n          ],\n          \"managementZones\": [\n            {\n              \"id\": \"abc123\",\n              \"name\": \"Production Service\"\n            }\n          ],\n          \"toRelationships\": {},\n          \"fromRelationships\": {}\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/entities-api-v2-entity-collection-schema.json
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
title: EntityCollection
---
