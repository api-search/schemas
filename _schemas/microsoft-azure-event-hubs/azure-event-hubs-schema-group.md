---
description: A schema group is a logical grouping of schemas within the Event Hubs Schema Registry. Schema groups define the serialization type (e.g., Avro) and compatibility mode (e.g., Backward, Forward) for schemas registered within the group. The Schema Registry enables schema-driven event serialization and deserialization for Event Hubs producers and consumers.
layout: schema
name: Azure Event Hubs Schema Group
properties_list:
- description: Fully qualified resource ID for the resource.
  name: id
  type: string
- description: The name of the schema group.
  name: name
  type: string
- description: The type of the resource.
  name: type
  type: string
- description: Schema group properties.
  name: properties
  type: object
- description: Metadata pertaining to creation and last modification of the resource.
  name: systemData
  type: object
provider_name: Azure Event Hubs
provider_slug: microsoft-azure-event-hubs
schema_file: json-schema/azure-event-hubs-schema-group.json
slug: azure-event-hubs-schema-group
source_filename: azure-event-hubs-schema-group.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.azure.com/eventhub/2024-01-01/schema-group.json\",\n  \"title\": \"Azure Event Hubs Schema Group\",\n  \"description\": \"A schema group is a logical grouping of schemas within the Event Hubs Schema Registry. Schema groups define the serialization type (e.g., Avro) and compatibility mode (e.g., Backward, Forward) for schemas registered within the group. The Schema Registry enables schema-driven event serialization and deserialization for Event Hubs producers and consumers.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified resource ID for the resource.\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the schema group.\",\n      \"minLength\": 1,\n      \"maxLength\": 256,\n      \"readOnly\": true\n    },\n    \"type\": {\n \
  \     \"type\": \"string\",\n      \"description\": \"The type of the resource.\",\n      \"const\": \"Microsoft.EventHub/Namespaces/SchemaGroups\",\n      \"readOnly\": true\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Schema group properties.\",\n      \"properties\": {\n        \"updatedAtUtc\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Exact time the Schema Group was updated.\",\n          \"readOnly\": true\n        },\n        \"createdAtUtc\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Exact time the Schema Group was created.\",\n          \"readOnly\": true\n        },\n        \"eTag\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The ETag value.\",\n          \"readOnly\": true\n        },\n        \"groupProperties\": {\n          \"type\": \"object\",\n         \
  \ \"additionalProperties\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Dictionary object for SchemaGroup group properties.\"\n        },\n        \"schemaCompatibility\": {\n          \"type\": \"string\",\n          \"description\": \"Schema compatibility setting that determines what changes are allowed when registering new schema versions.\",\n          \"enum\": [\"None\", \"Backward\", \"Forward\"]\n        },\n        \"schemaType\": {\n          \"type\": \"string\",\n          \"description\": \"Schema serialization type used by schemas in this group.\",\n          \"enum\": [\"Unknown\", \"Avro\"]\n        }\n      }\n    },\n    \"systemData\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata pertaining to creation and last modification of the resource.\",\n      \"properties\": {\n        \"createdBy\": {\n          \"type\": \"string\"\n        },\n        \"createdByType\": {\n          \"type\": \"string\",\n          \"\
  enum\": [\"User\", \"Application\", \"ManagedIdentity\", \"Key\"]\n        },\n        \"createdAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"lastModifiedBy\": {\n          \"type\": \"string\"\n        },\n        \"lastModifiedByType\": {\n          \"type\": \"string\",\n          \"enum\": [\"User\", \"Application\", \"ManagedIdentity\", \"Key\"]\n        },\n        \"lastModifiedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-event-hubs/refs/heads/main/json-schema/azure-event-hubs-schema-group.json
tags:
- Big Data
- Event Streaming
- IoT
- Message Ingestion
- Real-Time Processing
title: Azure Event Hubs Schema Group
---
