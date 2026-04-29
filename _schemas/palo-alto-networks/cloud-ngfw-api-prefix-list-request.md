---
description: PrefixListRequest schema from Palo Alto Networks Cloud NGFW for AWS REST API
layout: schema
name: PrefixListRequest
properties_list:
- description: ''
  name: PrefixListName
  type: string
- description: ''
  name: PrefixListEntry
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cloud-ngfw-api-prefix-list-request-schema.json
slug: cloud-ngfw-api-prefix-list-request
source_filename: cloud-ngfw-api-prefix-list-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PrefixListRequest\",\n  \"description\": \"PrefixListRequest schema from Palo Alto Networks Cloud NGFW for AWS REST API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-ngfw-api-prefix-list-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PrefixListName\": {\n      \"type\": \"string\"\n    },\n    \"PrefixListEntry\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"PrefixList\"\n      ],\n      \"properties\": {\n        \"Description\": {\n          \"type\": \"string\"\n        },\n        \"PrefixList\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"PrefixListName\",\n    \"PrefixListEntry\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-ngfw-api-prefix-list-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: PrefixListRequest
---
