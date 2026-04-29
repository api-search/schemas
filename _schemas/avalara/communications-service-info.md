---
description: ServiceInfo schema from Avalara API
layout: schema
name: ServiceInfo
properties_list:
- description: ''
  name: serverTime
  type: string
- description: ''
  name: buildVersion
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/communications-service-info-schema.json
slug: communications-service-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-service-info-schema.json\",\n  \"title\": \"ServiceInfo\",\n  \"description\": \"ServiceInfo schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serverTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"buildVersion\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-service-info-schema.json
tags:
- Taxes
title: ServiceInfo
---
