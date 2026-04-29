---
description: An Experience Data Model (XDM) event object.
layout: schema
name: XDMEvent
properties_list:
- description: A map of identity namespaces to arrays of identity objects for cross-device identity stitching.
  name: identityMap
  type: object
- description: The type of event (e.g., web.webpagedetails.pageViews, commerce.productViews, commerce.purchases).
  name: eventType
  type: string
- description: Web-specific event data.
  name: web
  type: object
- description: Commerce-specific event data.
  name: commerce
  type: object
- description: The ISO 8601 timestamp of the event.
  name: timestamp
  type: string
provider_name: Adobe Launch
provider_slug: adobe-launch
schema_file: json-schema/data-collection-xdm-event-schema.json
slug: data-collection-xdm-event
source_filename: data-collection-xdm-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"XDMEvent\",\n  \"type\": \"object\",\n  \"description\": \"An Experience Data Model (XDM) event object.\",\n  \"properties\": {\n    \"identityMap\": {\n      \"type\": \"object\",\n      \"description\": \"A map of identity namespaces to arrays of identity objects for cross-device identity stitching.\"\n    },\n    \"eventType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of event (e.g., web.webpagedetails.pageViews, commerce.productViews, commerce.purchases).\"\n    },\n    \"web\": {\n      \"type\": \"object\",\n      \"description\": \"Web-specific event data.\"\n    },\n    \"commerce\": {\n      \"type\": \"object\",\n      \"description\": \"Commerce-specific event data.\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO 8601 timestamp of the event.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/json-schema/data-collection-xdm-event-schema.json
tags:
- Data Collection
- Edge Network
- Event Forwarding
- Marketing Technology
- Tag Management
title: XDMEvent
---
