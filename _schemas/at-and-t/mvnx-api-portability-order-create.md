---
description: PortabilityOrderCreate schema from AT&T API
layout: schema
name: PortabilityOrderCreate
properties_list:
- description: ''
  name: portabilityOrderItem
  type: array
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/mvnx-api-portability-order-create-schema.json
slug: mvnx-api-portability-order-create
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-portability-order-create-schema.json\",\n  \"title\": \"PortabilityOrderCreate\",\n  \"description\": \"PortabilityOrderCreate schema from AT&T API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"portabilityOrderItem\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"msisdn\": {\n            \"type\": \"string\",\n            \"description\": \"Phone number to port\",\n            \"example\": \"+12125551234\"\n          },\n          \"portingType\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"FULL\",\n              \"PARTIAL\"\n            ],\n            \"example\": \"FULL\"\n          },\n          \"currentCarrier\": {\n            \"type\": \"string\",\n            \"description\"\
  : \"Current carrier name\",\n            \"example\": \"Verizon\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-portability-order-create-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: PortabilityOrderCreate
---
