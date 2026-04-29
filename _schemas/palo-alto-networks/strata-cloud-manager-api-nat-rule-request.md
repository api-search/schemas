---
description: NatRuleRequest schema from Palo Alto Networks Strata Cloud Manager API
layout: schema
name: NatRuleRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: from
  type: array
- description: ''
  name: to
  type: array
- description: ''
  name: source
  type: array
- description: ''
  name: destination
  type: array
- description: ''
  name: service
  type: string
- description: ''
  name: source_translation
  type: object
- description: ''
  name: destination_translation
  type: object
- description: ''
  name: disabled
  type: boolean
- description: ''
  name: description
  type: string
- description: ''
  name: tag
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/strata-cloud-manager-api-nat-rule-request-schema.json
slug: strata-cloud-manager-api-nat-rule-request
source_filename: strata-cloud-manager-api-nat-rule-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NatRuleRequest\",\n  \"description\": \"NatRuleRequest schema from Palo Alto Networks Strata Cloud Manager API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-cloud-manager-api-nat-rule-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"from\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"to\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"source\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"destination\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"service\": {\n      \"type\": \"string\"\n    },\n    \"source_translation\"\
  : {\n      \"type\": \"object\",\n      \"properties\": {\n        \"dynamic_ip_and_port\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"translated_address\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        },\n        \"static_ip\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"translated_address\": {\n              \"type\": \"string\"\n            },\n            \"bi_directional\": {\n              \"type\": \"boolean\"\n            }\n          }\n        }\n      }\n    },\n    \"destination_translation\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"translated_address\": {\n          \"type\": \"string\"\n        },\n        \"translated_port\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"disabled\": {\n      \"type\": \"boolean\"\n    },\n    \"description\"\
  : {\n      \"type\": \"string\"\n    },\n    \"tag\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-cloud-manager-api-nat-rule-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: NatRuleRequest
---
