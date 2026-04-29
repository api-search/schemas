---
description: An IP prefix list containing CIDR entries for use in security rule source and destination criteria.
layout: schema
name: PrefixList
properties_list:
- description: ''
  name: PrefixListName
  type: string
- description: ''
  name: PrefixListEntry
  type: object
- description: ''
  name: UpdateToken
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cloud-ngfw-api-prefix-list-schema.json
slug: cloud-ngfw-api-prefix-list
source_filename: cloud-ngfw-api-prefix-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PrefixList\",\n  \"description\": \"An IP prefix list containing CIDR entries for use in security rule source and destination criteria.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-ngfw-api-prefix-list-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PrefixListName\": {\n      \"type\": \"string\"\n    },\n    \"PrefixListEntry\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Description\": {\n          \"type\": \"string\"\n        },\n        \"PrefixList\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"CIDR block entries (e.g., 10.0.0.0/8, 192.168.0.0/16).\"\n        }\n      }\n    },\n    \"UpdateToken\": {\n      \"type\": \"string\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-ngfw-api-prefix-list-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: PrefixList
---
