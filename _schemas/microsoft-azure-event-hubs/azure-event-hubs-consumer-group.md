---
description: A consumer group is a view (state, position, or offset) of an entire event hub. Consumer groups enable multiple consuming applications to each have a separate view of the event stream, and to read the stream independently at their own pace and with their own offsets. A default consumer group ($Default) is automatically created for each event hub.
layout: schema
name: Azure Event Hubs Consumer Group
properties_list:
- description: Fully qualified resource ID for the resource.
  name: id
  type: string
- description: The name of the consumer group.
  name: name
  type: string
- description: The type of the resource.
  name: type
  type: string
- description: The geo-location where the resource lives.
  name: location
  type: string
- description: Consumer group properties.
  name: properties
  type: object
- description: Metadata pertaining to creation and last modification of the resource.
  name: systemData
  type: object
provider_name: Azure Event Hubs
provider_slug: microsoft-azure-event-hubs
schema_file: json-schema/azure-event-hubs-consumer-group.json
slug: azure-event-hubs-consumer-group
source_filename: azure-event-hubs-consumer-group.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.azure.com/eventhub/2024-01-01/consumer-group.json\",\n  \"title\": \"Azure Event Hubs Consumer Group\",\n  \"description\": \"A consumer group is a view (state, position, or offset) of an entire event hub. Consumer groups enable multiple consuming applications to each have a separate view of the event stream, and to read the stream independently at their own pace and with their own offsets. A default consumer group ($Default) is automatically created for each event hub.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified resource ID for the resource.\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the consumer group.\",\n      \"minLength\": 1,\n      \"maxLength\": 50,\n      \"readOnly\": true\n    },\n    \"type\": {\n   \
  \   \"type\": \"string\",\n      \"description\": \"The type of the resource.\",\n      \"const\": \"Microsoft.EventHub/Namespaces/EventHubs/ConsumerGroups\",\n      \"readOnly\": true\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"The geo-location where the resource lives.\",\n      \"readOnly\": true\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Consumer group properties.\",\n      \"properties\": {\n        \"createdAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Exact time the consumer group was created.\",\n          \"readOnly\": true\n        },\n        \"updatedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The exact time the consumer group was last updated.\",\n          \"readOnly\": true\n        },\n        \"userMetadata\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"User Metadata is a placeholder to store user-defined string data with maximum length 1024. It can be used to store descriptive data, such as list of teams and their contact information, or user-defined configuration settings.\",\n          \"maxLength\": 1024\n        }\n      }\n    },\n    \"systemData\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata pertaining to creation and last modification of the resource.\",\n      \"properties\": {\n        \"createdBy\": {\n          \"type\": \"string\"\n        },\n        \"createdByType\": {\n          \"type\": \"string\",\n          \"enum\": [\"User\", \"Application\", \"ManagedIdentity\", \"Key\"]\n        },\n        \"createdAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"lastModifiedBy\": {\n          \"type\": \"string\"\n        },\n        \"lastModifiedByType\": {\n          \"type\": \"string\",\n          \"enum\": [\"User\", \"Application\", \"ManagedIdentity\"\
  , \"Key\"]\n        },\n        \"lastModifiedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-event-hubs/refs/heads/main/json-schema/azure-event-hubs-consumer-group.json
tags:
- Big Data
- Event Streaming
- IoT
- Message Ingestion
- Real-Time Processing
title: Azure Event Hubs Consumer Group
---
