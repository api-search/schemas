---
description: Represents a single event instance that occurred in the system
layout: schema
name: EventInstance
properties_list:
- description: Unique identifier for the event instance
  name: id
  type: string
- description: The type of event that occurred
  name: eventType
  type: string
- description: The ID of the CRM object associated with this event
  name: objectId
  type: string
- description: The type of CRM object (e.g., contact, company, deal)
  name: objectType
  type: string
- description: ISO 8601 timestamp when the event occurred
  name: occurredAt
  type: string
- description: Additional properties associated with the event
  name: properties
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/analytics-events-api-event-instance-schema.json
slug: analytics-events-api-event-instance
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/analytics-events-api-event-instance-schema.json\",\n  \"title\": \"EventInstance\",\n  \"description\": \"Represents a single event instance that occurred in the system\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the event instance\",\n      \"example\": \"500123\"\n    },\n    \"eventType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of event that occurred\",\n      \"example\": \"standard\"\n    },\n    \"objectId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the CRM object associated with this event\",\n      \"example\": \"500123\"\n    },\n    \"objectType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of CRM object (e.g., contact, company, deal)\"\
  ,\n      \"example\": \"standard\"\n    },\n    \"occurredAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the event occurred\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Additional properties associated with the event\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"eventType\",\n    \"occurredAt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/analytics-events-api-event-instance-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: EventInstance
---
