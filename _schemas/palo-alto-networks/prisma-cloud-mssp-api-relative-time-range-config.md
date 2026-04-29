---
description: 'RelativeTimeRangeConfig schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: RelativeTimeRangeConfig
properties_list: []
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-relative-time-range-config-schema.json
slug: prisma-cloud-mssp-api-relative-time-range-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RelativeTimeRangeConfig\",\n  \"description\": \"RelativeTimeRangeConfig schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-relative-time-range-config-schema.json\",\n  \"type\": \"object\",\n  \"allOf\": [\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\"\n        },\n        \"timeUnit\": {\n          \"type\": \"string\"\n        },\n        \"timeValue\": {\n          \"type\": \"integer\",\n          \"format\": \"int32\"\n        }\n      },\n      \"discriminator\": {\n        \"propertyName\": \"type\"\n      }\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"value\": {\n          \"type\": \"object\",\n          \"properties\": {\n         \
  \   \"unit\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"week\",\n                \"month\",\n                \"year\"\n              ]\n            },\n            \"amount\": {\n              \"type\": \"integer\",\n              \"description\": \"Number of time units\",\n              \"format\": \"int32\"\n            }\n          }\n        }\n      }\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-relative-time-range-config-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: RelativeTimeRangeConfig
---
