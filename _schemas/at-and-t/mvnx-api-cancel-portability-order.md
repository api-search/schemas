---
description: CancelPortabilityOrder schema from AT&T API
layout: schema
name: CancelPortabilityOrder
properties_list:
- description: ''
  name: portabilityOrder
  type: object
- description: Reason for cancellation
  name: cancellationReason
  type: string
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/mvnx-api-cancel-portability-order-schema.json
slug: mvnx-api-cancel-portability-order
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-cancel-portability-order-schema.json\",\n  \"title\": \"CancelPortabilityOrder\",\n  \"description\": \"CancelPortabilityOrder schema from AT&T API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"portabilityOrder\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Port order ID to cancel\",\n          \"example\": \"port-500123\"\n        }\n      }\n    },\n    \"cancellationReason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason for cancellation\",\n      \"example\": \"Customer request\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-cancel-portability-order-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: CancelPortabilityOrder
---
