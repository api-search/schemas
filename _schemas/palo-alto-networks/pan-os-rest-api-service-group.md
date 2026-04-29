---
description: A group of service objects for use in security policy rules.
layout: schema
name: ServiceGroup
properties_list:
- description: Unique name of the service group.
  name: '@name'
  type: string
- description: ''
  name: members
  type: object
- description: ''
  name: tag
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/pan-os-rest-api-service-group-schema.json
slug: pan-os-rest-api-service-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceGroup\",\n  \"description\": \"A group of service objects for use in security policy rules.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/pan-os-rest-api-service-group-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name of the service group.\"\n    },\n    \"members\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"member\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"List of service object names.\"\n        }\n      }\n    },\n    \"tag\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"member\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n        \
  \  }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/pan-os-rest-api-service-group-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ServiceGroup
---
