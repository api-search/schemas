---
description: Collection of available event type names
layout: schema
name: EventTypeCollection
properties_list:
- description: List of available event type names
  name: eventTypes
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/analytics-events-api-event-type-collection-schema.json
slug: analytics-events-api-event-type-collection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/analytics-events-api-event-type-collection-schema.json\",\n  \"title\": \"EventTypeCollection\",\n  \"description\": \"Collection of available event type names\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventTypes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of available event type names\",\n      \"example\": [\n        \"standard\"\n      ]\n    }\n  },\n  \"required\": [\n    \"eventTypes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/analytics-events-api-event-type-collection-schema.json
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
title: EventTypeCollection
---
