---
description: AddressGroupRequest schema from Palo Alto Networks Strata Cloud Manager API
layout: schema
name: AddressGroupRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: static
  type: array
- description: ''
  name: dynamic
  type: object
- description: ''
  name: description
  type: string
- description: ''
  name: tag
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/strata-cloud-manager-api-address-group-request-schema.json
slug: strata-cloud-manager-api-address-group-request
source_filename: strata-cloud-manager-api-address-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AddressGroupRequest\",\n  \"description\": \"AddressGroupRequest schema from Palo Alto Networks Strata Cloud Manager API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-cloud-manager-api-address-group-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"static\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"dynamic\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"filter\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"tag\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-cloud-manager-api-address-group-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: AddressGroupRequest
---
