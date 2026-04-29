---
description: FqdnListRequest schema from Palo Alto Networks Cloud NGFW for AWS REST API
layout: schema
name: FqdnListRequest
properties_list:
- description: ''
  name: FqdnListName
  type: string
- description: ''
  name: FqdnListEntry
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cloud-ngfw-api-fqdn-list-request-schema.json
slug: cloud-ngfw-api-fqdn-list-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FqdnListRequest\",\n  \"description\": \"FqdnListRequest schema from Palo Alto Networks Cloud NGFW for AWS REST API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-ngfw-api-fqdn-list-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FqdnListName\": {\n      \"type\": \"string\"\n    },\n    \"FqdnListEntry\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"FqdnList\"\n      ],\n      \"properties\": {\n        \"Description\": {\n          \"type\": \"string\"\n        },\n        \"FqdnList\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"FqdnListName\",\n    \"FqdnListEntry\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-ngfw-api-fqdn-list-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: FqdnListRequest
---
