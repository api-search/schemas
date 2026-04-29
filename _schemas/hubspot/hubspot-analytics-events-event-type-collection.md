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
schema_file: json-schema/hubspot-analytics-events-event-type-collection-schema.json
slug: hubspot-analytics-events-event-type-collection
source_filename: hubspot-analytics-events-event-type-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Collection of available event type names\",\n  \"properties\": {\n    \"eventTypes\": {\n      \"type\": \"array\",\n      \"description\": \"List of available event type names\",\n      \"example\": [\n        \"standard\"\n      ],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"eventTypes\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EventTypeCollection\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-analytics-events-event-type-collection-schema.json
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
