---
description: Status of a commit job.
layout: schema
name: CommitStatus
properties_list:
- description: ''
  name: '@status'
  type: string
- description: ''
  name: '@code'
  type: string
- description: ''
  name: result
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/pan-os-rest-api-commit-status-schema.json
slug: pan-os-rest-api-commit-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CommitStatus\",\n  \"description\": \"Status of a commit job.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/pan-os-rest-api-commit-status-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@status\": {\n      \"type\": \"string\"\n    },\n    \"@code\": {\n      \"type\": \"string\"\n    },\n    \"result\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"job\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"id\": {\n              \"type\": \"string\"\n            },\n            \"type\": {\n              \"type\": \"string\"\n            },\n            \"status\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"ACT\",\n                \"PEND\",\n                \"FIN\",\n                \"WARN\"\n              ]\n      \
  \      },\n            \"result\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"OK\",\n                \"FAIL\",\n                \"WARN\"\n              ]\n            },\n            \"progress\": {\n              \"type\": \"string\",\n              \"description\": \"Commit progress percentage (0-100).\"\n            },\n            \"details\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"line\": {\n                  \"oneOf\": [\n                    {\n                      \"type\": \"string\"\n                    },\n                    {\n                      \"type\": \"array\",\n                      \"items\": {\n                        \"type\": \"string\"\n                      }\n                    }\n                  ]\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/pan-os-rest-api-commit-status-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: CommitStatus
---
