---
description: Paginated collection of event instances
layout: schema
name: EventInstanceCollection
properties_list:
- description: Array of event instances
  name: results
  type: array
- description: Pagination information for navigating result sets
  name: paging
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-analytics-events-event-instance-collection-schema.json
slug: hubspot-analytics-events-event-instance-collection
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Paginated collection of event instances\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"Array of event instances\",\n      \"example\": [\n        {\n          \"id\": \"500123\",\n          \"eventType\": \"standard\",\n          \"objectId\": \"500123\",\n          \"objectType\": \"standard\",\n          \"occurredAt\": \"2025-03-15T14:30:00Z\",\n          \"properties\": {\n            \"key\": \"value\"\n          }\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Represents a single event instance that occurred in the system\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique identifier for the event instance\",\n            \"example\": \"500123\"\n          },\n          \"eventType\": {\n            \"type\": \"string\",\n            \"description\"\
  : \"The type of event that occurred\",\n            \"example\": \"standard\"\n          },\n          \"objectId\": {\n            \"type\": \"string\",\n            \"description\": \"The ID of the CRM object associated with this event\",\n            \"example\": \"500123\"\n          },\n          \"objectType\": {\n            \"type\": \"string\",\n            \"description\": \"The type of CRM object (e.g., contact, company, deal)\",\n            \"example\": \"standard\"\n          },\n          \"occurredAt\": {\n            \"type\": \"string\",\n            \"description\": \"ISO 8601 timestamp when the event occurred\",\n            \"format\": \"date-time\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"properties\": {\n            \"type\": \"object\",\n            \"description\": \"Additional properties associated with the event\",\n            \"example\": {\n              \"key\": \"value\"\n            }\n          }\n        },\n    \
  \    \"required\": [\n          \"id\",\n          \"eventType\",\n          \"occurredAt\"\n        ]\n      }\n    },\n    \"paging\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination information for navigating result sets\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"object\",\n          \"description\": \"Pagination cursor for retrieving the next page of results\",\n          \"properties\": {\n            \"after\": {\n              \"type\": \"string\",\n              \"description\": \"Cursor token for the next page\",\n              \"example\": \"example-value\"\n            },\n            \"link\": {\n              \"type\": \"string\",\n              \"description\": \"API link to the next page of results\",\n              \"example\": \"https://app.hubspot.com/contacts/12345\"\n            }\n          }\n        },\n        \"prev\": {\n          \"type\": \"object\",\n          \"description\": \"Pagination cursor for retrieving\
  \ the previous page of results\",\n          \"properties\": {\n            \"before\": {\n              \"type\": \"string\",\n              \"description\": \"Cursor token for the previous page\",\n              \"example\": \"example-value\"\n            },\n            \"link\": {\n              \"type\": \"string\",\n              \"description\": \"API link to the previous page of results\",\n              \"example\": \"https://app.hubspot.com/contacts/12345\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"results\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EventInstanceCollection\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-analytics-events-event-instance-collection-schema.json
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
title: EventInstanceCollection
---
