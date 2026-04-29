---
description: PortabilityOrderCancellation schema from AT&T API
layout: schema
name: PortabilityOrderCancellation
properties_list:
- description: Cancellation record ID
  name: id
  type: string
- description: Cancellation state
  name: state
  type: string
- description: ''
  name: portabilityOrder
  type: object
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/mvnx-api-portability-order-cancellation-schema.json
slug: mvnx-api-portability-order-cancellation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-portability-order-cancellation-schema.json\",\n  \"title\": \"PortabilityOrderCancellation\",\n  \"description\": \"PortabilityOrderCancellation schema from AT&T API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Cancellation record ID\",\n      \"example\": \"cancel-500123\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Cancellation state\",\n      \"example\": \"completed\"\n    },\n    \"portabilityOrder\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"port-500123\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-portability-order-cancellation-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: PortabilityOrderCancellation
---
