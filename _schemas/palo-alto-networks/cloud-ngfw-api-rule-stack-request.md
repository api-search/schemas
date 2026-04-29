---
description: RuleStackRequest schema from Palo Alto Networks Cloud NGFW for AWS REST API
layout: schema
name: RuleStackRequest
properties_list:
- description: ''
  name: RuleStackName
  type: string
- description: ''
  name: RuleStackEntry
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cloud-ngfw-api-rule-stack-request-schema.json
slug: cloud-ngfw-api-rule-stack-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RuleStackRequest\",\n  \"description\": \"RuleStackRequest schema from Palo Alto Networks Cloud NGFW for AWS REST API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-ngfw-api-rule-stack-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RuleStackName\": {\n      \"type\": \"string\"\n    },\n    \"RuleStackEntry\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Description\": {\n          \"type\": \"string\"\n        },\n        \"Scope\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"Local\",\n            \"Global\"\n          ],\n          \"default\": \"Local\"\n        },\n        \"MinAppIdVersion\": {\n          \"type\": \"string\"\n        },\n        \"Profile\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"\
  AntiSpywareProfile\": {\n              \"type\": \"string\"\n            },\n            \"AntiVirusProfile\": {\n              \"type\": \"string\"\n            },\n            \"VulnerabilityProfile\": {\n              \"type\": \"string\"\n            },\n            \"URLFilteringProfile\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"RuleStackName\",\n    \"RuleStackEntry\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-ngfw-api-rule-stack-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: RuleStackRequest
---
