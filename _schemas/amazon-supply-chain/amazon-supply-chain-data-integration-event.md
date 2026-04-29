---
description: A data integration event
layout: schema
name: DataIntegrationEvent
properties_list:
- description: The instance identifier
  name: instanceId
  type: string
- description: The event identifier
  name: eventId
  type: string
- description: The event type
  name: eventType
  type: string
- description: The event group identifier
  name: eventGroupId
  type: string
- description: The event timestamp
  name: eventTimestamp
  type: string
- description: The event data payload
  name: data
  type: string
provider_name: Amazon Supply Chain
provider_slug: amazon-supply-chain
schema_file: json-schema/amazon-supply-chain-data-integration-event-schema.json
slug: amazon-supply-chain-data-integration-event
source_filename: amazon-supply-chain-data-integration-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-supply-chain/refs/heads/main/json-schema/amazon-supply-chain-data-integration-event-schema.json\",\n  \"title\": \"DataIntegrationEvent\",\n  \"description\": \"A data integration event\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instanceId\": {\n      \"type\": \"string\",\n      \"description\": \"The instance identifier\"\n    },\n    \"eventId\": {\n      \"type\": \"string\",\n      \"description\": \"The event identifier\"\n    },\n    \"eventType\": {\n      \"type\": \"string\",\n      \"description\": \"The event type\"\n    },\n    \"eventGroupId\": {\n      \"type\": \"string\",\n      \"description\": \"The event group identifier\"\n    },\n    \"eventTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The event timestamp\"\n    },\n    \"data\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"The event data payload\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-supply-chain/refs/heads/main/json-schema/amazon-supply-chain-data-integration-event-schema.json
tags:
- AWS
- ERP Integration
- Logistics
- Machine Learning
- Supply Chain
title: DataIntegrationEvent
---
