---
description: Event schema from ARGUS Enterprise API
layout: schema
name: Event
properties_list:
- description: Unique event identifier
  name: id
  type: string
- description: Subscription that received this event
  name: subscriptionId
  type: string
- description: Type of event
  name: eventType
  type: string
- description: Delivery status
  name: status
  type: string
- description: Event payload data
  name: payload
  type: object
- description: ''
  name: deliveryAttempts
  type: array
- description: ''
  name: createdAt
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-event-schema.json
slug: argus-enterprise-event
source_filename: argus-enterprise-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-event-schema.json\",\n  \"title\": \"Event\",\n  \"description\": \"Event schema from ARGUS Enterprise API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique event identifier\"\n    },\n    \"subscriptionId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Subscription that received this event\"\n    },\n    \"eventType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of event\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Pending\",\n        \"Delivered\",\n        \"Failed\",\n        \"Retrying\"\n      ],\n      \"description\": \"Delivery status\"\n    },\n    \"payload\": {\n      \"\
  type\": \"object\",\n      \"description\": \"Event payload data\",\n      \"properties\": {\n        \"eventId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        },\n        \"eventType\": {\n          \"type\": \"string\"\n        },\n        \"timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"resourceType\": {\n          \"type\": \"string\",\n          \"description\": \"Type of resource that triggered the event\"\n        },\n        \"resourceId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"Identifier of the resource\"\n        },\n        \"data\": {\n          \"type\": \"object\",\n          \"description\": \"Resource data at the time of the event\"\n        }\n      }\n    },\n    \"deliveryAttempts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DeliveryAttempt\"\n      }\n    },\n    \"createdAt\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-event-schema.json
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: Event
---
