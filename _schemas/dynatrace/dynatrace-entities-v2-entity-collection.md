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
schema_file: json-schema/dynatrace-entities-v2-entity-collection-schema.json
slug: dynatrace-entities-v2-entity-collection
source_filename: dynatrace-entities-v2-entity-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A paginated collection of monitored entities.\",\n  \"properties\": {\n    \"nextPageKey\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor for the next page of results. Null if no more pages.\",\n      \"example\": \"example-value\"\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of entities matching the query.\",\n      \"format\": \"int64\",\n      \"example\": 500\n    },\n    \"pageSize\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of results returned on this page.\",\n      \"example\": 500\n    },\n    \"entities\": {\n      \"type\": \"array\",\n      \"description\": \"The list of entities on this page.\",\n      \"example\": [\n        {\n          \"entityId\": \"abc123\",\n          \"displayName\": \"Production Service\",\n          \"type\": \"STANDARD\",\n          \"firstSeenTms\": 500,\n          \"lastSeenTms\"\
  : 500,\n          \"properties\": {},\n          \"tags\": [\n            {\n              \"context\": \"example-value\",\n              \"key\": \"example-value\",\n              \"value\": \"example-value\",\n              \"stringRepresentation\": \"example-value\"\n            }\n          ],\n          \"managementZones\": [\n            {\n              \"id\": \"abc123\",\n              \"name\": \"Production Service\"\n            }\n          ],\n          \"toRelationships\": {},\n          \"fromRelationships\": {}\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Represents a monitored entity in Dynatrace. Entities are the components of your monitored environment such as services, hosts, processes, and applications. Each entity has a unique ID, a type, properties, tags, and relationships to other entities.\",\n        \"properties\": {\n          \"entityId\": {\n            \"type\": \"string\",\n            \"description\"\
  : \"The unique identifier of the entity in the format TYPE-HEXADECIMALID, e.g., SERVICE-1234567890ABCDEF.\",\n            \"example\": \"abc123\"\n          },\n          \"displayName\": {\n            \"type\": \"string\",\n            \"description\": \"The human-readable display name of the entity.\",\n            \"example\": \"Production Service\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"The type of the entity, e.g., SERVICE, HOST, PROCESS_GROUP, APPLICATION, SYNTHETIC_TEST.\",\n            \"example\": \"STANDARD\"\n          },\n          \"firstSeenTms\": {\n            \"type\": \"integer\",\n            \"description\": \"The Unix timestamp in milliseconds when the entity was first seen.\",\n            \"format\": \"int64\",\n            \"example\": 500\n          },\n          \"lastSeenTms\": {\n            \"type\": \"integer\",\n            \"description\": \"The Unix timestamp in milliseconds when the entity\
  \ was last seen.\",\n            \"format\": \"int64\",\n            \"example\": 500\n          },\n          \"properties\": {\n            \"type\": \"object\",\n            \"description\": \"A map of entity-type-specific properties. Available properties vary by entity type. For example, a HOST entity may include osType, cpuCores, and memoryTotalBytes.\",\n            \"example\": {}\n          },\n          \"tags\": {\n            \"type\": \"array\",\n            \"description\": \"The list of tags applied to the entity, including auto-detected and manually defined tags.\",\n            \"example\": [\n              {\n                \"context\": \"example-value\",\n                \"key\": \"example-value\",\n                \"value\": \"example-value\",\n                \"stringRepresentation\": \"example-value\"\n              }\n            ],\n            \"items\": {\n              \"type\": \"object\",\n              \"description\": \"A tag applied to a monitored entity.\"\
  ,\n              \"properties\": {\n                \"context\": {\n                  \"type\": \"string\",\n                  \"description\": \"The origin context of the tag. For example, CONTEXTLESS, ENVIRONMENT, AWS, KUBERNETES, etc.\",\n                  \"example\": \"example-value\"\n                },\n                \"key\": {\n                  \"type\": \"string\",\n                  \"description\": \"The key of the tag.\",\n                  \"example\": \"example-value\"\n                },\n                \"value\": {\n                  \"type\": \"string\",\n                  \"description\": \"The value of the tag, if applicable.\",\n                  \"example\": \"example-value\"\n                },\n                \"stringRepresentation\": {\n                  \"type\": \"string\",\n                  \"description\": \"The full string representation of the tag as displayed in the Dynatrace UI, e.g., [KUBERNETES]app:my-service.\",\n                  \"example\": \"\
  example-value\"\n                }\n              }\n            }\n          },\n          \"managementZones\": {\n            \"type\": \"array\",\n            \"description\": \"The management zones that the entity belongs to, used for access control and organizational scoping.\",\n            \"example\": [\n              {\n                \"id\": \"abc123\",\n                \"name\": \"Production Service\"\n              }\n            ],\n            \"items\": {\n              \"type\": \"object\",\n              \"description\": \"A management zone reference.\",\n              \"properties\": {\n                \"id\": {\n                  \"type\": \"string\",\n                  \"description\": \"The unique identifier of the management zone.\",\n                  \"example\": \"abc123\"\n                },\n                \"name\": {\n                  \"type\": \"string\",\n                  \"description\": \"The display name of the management zone.\",\n                \
  \  \"example\": \"Production Service\"\n                }\n              }\n            }\n          },\n          \"toRelationships\": {\n            \"type\": \"object\",\n            \"description\": \"Relationships where this entity is the target. Keys are relationship types (e.g., isProcessOf), values are arrays of entity IDs. For example, {\\\"isProcessOf\\\": [\\\"PROCESS_GROUP-123\\\"]}.\",\n            \"example\": {}\n          },\n          \"fromRelationships\": {\n            \"type\": \"object\",\n            \"description\": \"Relationships where this entity is the source. Keys are relationship types (e.g., runsOn), values are arrays of entity IDs. For example, {\\\"runsOn\\\": [\\\"HOST-456\\\"]}.\",\n            \"example\": {}\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EntityCollection\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-entities-v2-entity-collection-schema.json
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
