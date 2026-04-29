---
description: SubnetRuleRequest schema from Palo Alto Networks ZTNA Connector API
layout: schema
name: SubnetRuleRequest
properties_list:
- description: Display name for the subnet rule.
  name: name
  type: string
- description: CIDR notation subnet this rule covers.
  name: subnet
  type: string
- description: Connector group to use for routing traffic to this subnet.
  name: group_id
  type: string
- description: ''
  name: enabled
  type: boolean
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/ztna-connector-api-subnet-rule-request-schema.json
slug: ztna-connector-api-subnet-rule-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SubnetRuleRequest\",\n  \"description\": \"SubnetRuleRequest schema from Palo Alto Networks ZTNA Connector API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/ztna-connector-api-subnet-rule-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the subnet rule.\"\n    },\n    \"subnet\": {\n      \"type\": \"string\",\n      \"description\": \"CIDR notation subnet this rule covers.\"\n    },\n    \"group_id\": {\n      \"type\": \"string\",\n      \"description\": \"Connector group to use for routing traffic to this subnet.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"default\": true\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"subnet\",\n    \"group_id\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/ztna-connector-api-subnet-rule-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: SubnetRuleRequest
---
