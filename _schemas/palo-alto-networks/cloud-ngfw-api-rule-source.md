---
description: Traffic source matching criteria for a security rule.
layout: schema
name: RuleSource
properties_list:
- description: Source CIDR blocks (e.g., 10.0.0.0/8).
  name: Cidrs
  type: array
- description: Source country codes (ISO 3166-1 alpha-2).
  name: Countries
  type: array
- description: Threat intelligence feed names.
  name: Feeds
  type: array
- description: Names of prefix lists defined in the rule stack.
  name: PrefixLists
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cloud-ngfw-api-rule-source-schema.json
slug: cloud-ngfw-api-rule-source
source_filename: cloud-ngfw-api-rule-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RuleSource\",\n  \"description\": \"Traffic source matching criteria for a security rule.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-ngfw-api-rule-source-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Cidrs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Source CIDR blocks (e.g., 10.0.0.0/8).\"\n    },\n    \"Countries\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Source country codes (ISO 3166-1 alpha-2).\"\n    },\n    \"Feeds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Threat intelligence feed names.\"\n    },\n    \"PrefixLists\": {\n      \"type\": \"array\",\n      \"items\"\
  : {\n        \"type\": \"string\"\n      },\n      \"description\": \"Names of prefix lists defined in the rule stack.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-ngfw-api-rule-source-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: RuleSource
---
