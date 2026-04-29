---
description: RuleStackSummary schema from Palo Alto Networks Cloud NGFW for AWS REST API
layout: schema
name: RuleStackSummary
properties_list:
- description: ''
  name: RuleStackName
  type: string
- description: ''
  name: Scope
  type: string
- description: ''
  name: Status
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cloud-ngfw-api-rule-stack-summary-schema.json
slug: cloud-ngfw-api-rule-stack-summary
source_filename: cloud-ngfw-api-rule-stack-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RuleStackSummary\",\n  \"description\": \"RuleStackSummary schema from Palo Alto Networks Cloud NGFW for AWS REST API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-ngfw-api-rule-stack-summary-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RuleStackName\": {\n      \"type\": \"string\"\n    },\n    \"Scope\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Local\",\n        \"Global\"\n      ]\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"INACTIVE\",\n        \"ERROR\"\n      ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-ngfw-api-rule-stack-summary-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: RuleStackSummary
---
