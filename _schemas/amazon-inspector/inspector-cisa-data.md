---
description: The Cybersecurity and Infrastructure Security Agency (CISA) details for a specific vulnerability.
layout: schema
name: CisaData
properties_list:
- description: ''
  name: action
  type: object
- description: ''
  name: dateAdded
  type: object
- description: ''
  name: dateDue
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-cisa-data-schema.json
slug: inspector-cisa-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-cisa-data-schema.json\",\n  \"title\": \"CisaData\",\n  \"description\": \"The Cybersecurity and Infrastructure Security Agency (CISA) details for a specific vulnerability.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CisaAction\"\n        },\n        {\n          \"description\": \"The remediation action recommended by CISA for this vulnerability.\"\n        }\n      ]\n    },\n    \"dateAdded\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CisaDateAdded\"\n        },\n        {\n          \"description\": \"The date and time CISA added this vulnerability to their catalogue.\"\n        }\n      ]\n    },\n    \"dateDue\": {\n      \"allOf\": [\n        {\n      \
  \    \"$ref\": \"#/components/schemas/CisaDateDue\"\n        },\n        {\n          \"description\": \"The date and time CISA expects a fix to have been provided vulnerability.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-cisa-data-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: CisaData
---
