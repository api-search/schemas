---
description: A key-value metadata label applied to a FreeRTOS management resource.
layout: schema
name: Tag
properties_list:
- description: Tag key.
  name: key
  type: string
- description: Tag value.
  name: value
  type: string
provider_name: Amazon FreeRTOS
provider_slug: amazon-freertos
schema_file: json-schema/amazon-freertos-tag-schema.json
slug: amazon-freertos-tag
source_filename: amazon-freertos-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-freertos/refs/heads/main/json-schema/amazon-freertos-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"A key-value metadata label applied to a FreeRTOS management resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"Tag key.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Tag value.\"\n    }\n  },\n  \"required\": [\n    \"key\",\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-freertos/refs/heads/main/json-schema/amazon-freertos-tag-schema.json
tags:
- AWS
- Embedded Systems
- IoT
- Microcontrollers
- RTOS
title: Tag
---
