---
description: ResourceReservationCreate schema from AT&T API
layout: schema
name: ResourceReservationCreate
properties_list:
- description: ''
  name: resourceCapacity
  type: array
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/mvnx-api-resource-reservation-create-schema.json
slug: mvnx-api-resource-reservation-create
source_filename: mvnx-api-resource-reservation-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-resource-reservation-create-schema.json\",\n  \"title\": \"ResourceReservationCreate\",\n  \"description\": \"ResourceReservationCreate schema from AT&T API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceCapacity\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"resourcePool\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\",\n                \"example\": \"pool-212-area\"\n              }\n            }\n          },\n          \"capacityAmount\": {\n            \"type\": \"integer\",\n            \"example\": 1\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-resource-reservation-create-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: ResourceReservationCreate
---
