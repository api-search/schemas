---
description: FQDNRuleRequest schema from Palo Alto Networks ZTNA Connector API
layout: schema
name: FQDNRuleRequest
properties_list:
- description: Display name for the FQDN rule.
  name: name
  type: string
- description: FQDN pattern or wildcard this rule matches.
  name: fqdn_pattern
  type: string
- description: Connector group to use for matching FQDNs.
  name: group_id
  type: string
- description: Ports covered by this rule.
  name: ports
  type: array
- description: ''
  name: enabled
  type: boolean
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/ztna-connector-api-fqdn-rule-request-schema.json
slug: ztna-connector-api-fqdn-rule-request
source_filename: ztna-connector-api-fqdn-rule-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FQDNRuleRequest\",\n  \"description\": \"FQDNRuleRequest schema from Palo Alto Networks ZTNA Connector API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/ztna-connector-api-fqdn-rule-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the FQDN rule.\"\n    },\n    \"fqdn_pattern\": {\n      \"type\": \"string\",\n      \"description\": \"FQDN pattern or wildcard this rule matches.\"\n    },\n    \"group_id\": {\n      \"type\": \"string\",\n      \"description\": \"Connector group to use for matching FQDNs.\"\n    },\n    \"ports\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      },\n      \"description\": \"Ports covered by this rule.\"\n    },\n    \"enabled\": {\n      \"type\": \"\
  boolean\",\n      \"default\": true\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"fqdn_pattern\",\n    \"group_id\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/ztna-connector-api-fqdn-rule-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: FQDNRuleRequest
---
