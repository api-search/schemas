---
description: An FQDN list containing domain name entries for use in security rule destination criteria.
layout: schema
name: FqdnList
properties_list:
- description: ''
  name: FqdnListName
  type: string
- description: ''
  name: FqdnListEntry
  type: object
- description: ''
  name: UpdateToken
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cloud-ngfw-api-fqdn-list-schema.json
slug: cloud-ngfw-api-fqdn-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FqdnList\",\n  \"description\": \"An FQDN list containing domain name entries for use in security rule destination criteria.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-ngfw-api-fqdn-list-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FqdnListName\": {\n      \"type\": \"string\"\n    },\n    \"FqdnListEntry\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Description\": {\n          \"type\": \"string\"\n        },\n        \"FqdnList\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Fully qualified domain names (e.g., example.com, *.example.com).\"\n        }\n      }\n    },\n    \"UpdateToken\": {\n      \"type\": \"string\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-ngfw-api-fqdn-list-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: FqdnList
---
