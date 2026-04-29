---
description: A single meter event representing a unit of usage
layout: schema
name: MeterEvent
properties_list:
- description: The API name of the meter to ingest to
  name: meterApiName
  type: string
- description: Unique identifier for the customer
  name: customerId
  type: string
- description: The usage amount for this event
  name: meterValue
  type: number
- description: Event timestamp in Unix time (milliseconds)
  name: meterTimeInMillis
  type: integer
- description: Custom identifier for event deduplication
  name: uniqueId
  type: string
- description: Key-value pairs for event categorization
  name: dimensions
  type: object
- description: Map of meterApiName to meterValue for multi-meter ingestion
  name: values
  type: object
provider_name: Amberflo
provider_slug: amberflo
schema_file: json-schema/metering-meter-event-schema.json
slug: metering-meter-event
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/json-schema/metering-meter-event-schema.json\",\n  \"title\": \"MeterEvent\",\n  \"description\": \"A single meter event representing a unit of usage\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"meterApiName\": {\n      \"type\": \"string\",\n      \"description\": \"The API name of the meter to ingest to\",\n      \"example\": \"api-calls\"\n    },\n    \"customerId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the customer\",\n      \"example\": \"customer-123456\"\n    },\n    \"meterValue\": {\n      \"type\": \"number\",\n      \"description\": \"The usage amount for this event\",\n      \"example\": 1.0\n    },\n    \"meterTimeInMillis\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Event timestamp in Unix time (milliseconds)\"\
  ,\n      \"example\": 1718153645993\n    },\n    \"uniqueId\": {\n      \"type\": \"string\",\n      \"description\": \"Custom identifier for event deduplication\",\n      \"example\": \"evt-a1b2c3d4\"\n    },\n    \"dimensions\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Key-value pairs for event categorization\",\n      \"example\": {\n        \"region\": \"us-east-1\",\n        \"tier\": \"premium\"\n      }\n    },\n    \"values\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"number\"\n      },\n      \"description\": \"Map of meterApiName to meterValue for multi-meter ingestion\"\n    }\n  },\n  \"required\": [\n    \"meterTimeInMillis\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amberflo/refs/heads/main/json-schema/metering-meter-event-schema.json
tags:
- Usage-Based Billing
- Metering
- FinOps
- AI Cost Management
- Billing
- Monetization
title: MeterEvent
---
