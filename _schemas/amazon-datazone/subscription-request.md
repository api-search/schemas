---
description: A request to subscribe to a data asset listing in DataZone.
layout: schema
name: Subscription Request
properties_list:
- description: The unique identifier of the subscription request
  name: id
  type: string
- description: ''
  name: domainId
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: requestReason
  type: string
- description: ''
  name: createdAt
  type: string
provider_name: Amazon DataZone
provider_slug: amazon-datazone
schema_file: json-schema/subscription-request-schema.json
slug: subscription-request
source_filename: subscription-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-datazone/json-schema/subscription-request-schema.json\",\n  \"title\": \"Subscription Request\",\n  \"description\": \"A request to subscribe to a data asset listing in DataZone.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the subscription request\"\n    },\n    \"domainId\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PENDING\",\n        \"ACCEPTED\",\n        \"REJECTED\"\n      ]\n    },\n    \"requestReason\": {\n      \"type\": \"string\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-datazone/refs/heads/main/json-schema/subscription-request-schema.json
tags:
- Data Catalog
- Data Governance
- Data Management
- Data Sharing
- Analytics
title: Subscription Request
---
