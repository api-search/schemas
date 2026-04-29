---
description: RuntimePolicy schema from Palo Alto Networks Prisma Cloud Compute API
layout: schema
name: RuntimePolicy
properties_list:
- description: Container runtime defense rules.
  name: rules
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-compute-api-runtime-policy-schema.json
slug: prisma-cloud-compute-api-runtime-policy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RuntimePolicy\",\n  \"description\": \"RuntimePolicy schema from Palo Alto Networks Prisma Cloud Compute API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-compute-api-runtime-policy-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"rules\": {\n      \"type\": \"array\",\n      \"description\": \"Container runtime defense rules.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"collections\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"processes\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"effect\": {\n                \"type\": \"string\",\n     \
  \           \"enum\": [\n                  \"ignore\",\n                  \"alert\",\n                  \"block\"\n                ]\n              },\n              \"whitelist\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"string\"\n                }\n              },\n              \"blacklist\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          },\n          \"network\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"effect\": {\n                \"type\": \"string\",\n                \"enum\": [\n                  \"ignore\",\n                  \"alert\",\n                  \"block\"\n                ]\n              }\n            }\n          },\n          \"filesystem\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"effect\": {\n\
  \                \"type\": \"string\",\n                \"enum\": [\n                  \"ignore\",\n                  \"alert\",\n                  \"block\"\n                ]\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-compute-api-runtime-policy-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: RuntimePolicy
---
