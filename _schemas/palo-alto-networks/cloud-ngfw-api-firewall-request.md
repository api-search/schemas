---
description: FirewallRequest schema from Palo Alto Networks Cloud NGFW for AWS REST API
layout: schema
name: FirewallRequest
properties_list:
- description: ''
  name: FirewallName
  type: string
- description: ''
  name: FirewallEntry
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cloud-ngfw-api-firewall-request-schema.json
slug: cloud-ngfw-api-firewall-request
source_filename: cloud-ngfw-api-firewall-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FirewallRequest\",\n  \"description\": \"FirewallRequest schema from Palo Alto Networks Cloud NGFW for AWS REST API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-ngfw-api-firewall-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FirewallName\": {\n      \"type\": \"string\"\n    },\n    \"FirewallEntry\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"VpcId\",\n        \"AssociatedRuleStack\",\n        \"SubnetMappings\"\n      ],\n      \"properties\": {\n        \"Description\": {\n          \"type\": \"string\"\n        },\n        \"VpcId\": {\n          \"type\": \"string\"\n        },\n        \"AssociatedRuleStack\": {\n          \"type\": \"string\"\n        },\n        \"SubnetMappings\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\"\
  : \"object\",\n            \"properties\": {\n              \"SubnetId\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        },\n        \"Tags\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"Key\": {\n                \"type\": \"string\"\n              },\n              \"Value\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"FirewallName\",\n    \"FirewallEntry\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-ngfw-api-firewall-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: FirewallRequest
---
