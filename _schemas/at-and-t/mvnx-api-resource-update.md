---
description: ResourceUpdate schema from AT&T API
layout: schema
name: ResourceUpdate
properties_list:
- description: ''
  name: resourceCharacteristic
  type: array
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/mvnx-api-resource-update-schema.json
slug: mvnx-api-resource-update
source_filename: mvnx-api-resource-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-resource-update-schema.json\",\n  \"title\": \"ResourceUpdate\",\n  \"description\": \"ResourceUpdate schema from AT&T API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceCharacteristic\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Characteristic name to update\",\n            \"example\": \"voicemailPassword\"\n          },\n          \"value\": {\n            \"type\": \"string\",\n            \"description\": \"New value for the characteristic\",\n            \"example\": \"1234\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-resource-update-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: ResourceUpdate
---
