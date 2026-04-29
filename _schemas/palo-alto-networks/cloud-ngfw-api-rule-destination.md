---
description: Traffic destination matching criteria for a security rule.
layout: schema
name: RuleDestination
properties_list:
- description: Destination CIDR blocks.
  name: Cidrs
  type: array
- description: Destination country codes.
  name: Countries
  type: array
- description: ''
  name: Feeds
  type: array
- description: Names of FQDN lists defined in the rule stack.
  name: FqdnLists
  type: array
- description: ''
  name: PrefixLists
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cloud-ngfw-api-rule-destination-schema.json
slug: cloud-ngfw-api-rule-destination
source_filename: cloud-ngfw-api-rule-destination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RuleDestination\",\n  \"description\": \"Traffic destination matching criteria for a security rule.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-ngfw-api-rule-destination-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Cidrs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Destination CIDR blocks.\"\n    },\n    \"Countries\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Destination country codes.\"\n    },\n    \"Feeds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"FqdnLists\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Names of\
  \ FQDN lists defined in the rule stack.\"\n    },\n    \"PrefixLists\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-ngfw-api-rule-destination-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: RuleDestination
---
