---
description: PortabilityOrder schema from AT&T API
layout: schema
name: PortabilityOrder
properties_list:
- description: Unique port order identifier
  name: id
  type: string
- description: ''
  name: href
  type: string
- description: Port order state
  name: state
  type: string
- description: Requested completion date for the port
  name: requestedCompletionDate
  type: string
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/mvnx-api-portability-order-schema.json
slug: mvnx-api-portability-order
source_filename: mvnx-api-portability-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-portability-order-schema.json\",\n  \"title\": \"PortabilityOrder\",\n  \"description\": \"PortabilityOrder schema from AT&T API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique port order identifier\",\n      \"example\": \"port-500123\"\n    },\n    \"href\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://devex-web.att.com/portabilityOrder/port-500123\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Port order state\",\n      \"enum\": [\n        \"inProgress\",\n        \"completed\",\n        \"cancelled\",\n        \"failed\"\n      ],\n      \"example\": \"inProgress\"\n    },\n    \"requestedCompletionDate\": {\n      \"type\": \"string\",\n \
  \     \"format\": \"date-time\",\n      \"description\": \"Requested completion date for the port\",\n      \"example\": \"2026-04-25T00:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-portability-order-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: PortabilityOrder
---
