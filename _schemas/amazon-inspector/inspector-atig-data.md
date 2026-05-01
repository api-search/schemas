---
description: The Amazon Web Services Threat Intel Group (ATIG) details for a specific vulnerability.
layout: schema
name: AtigData
properties_list:
- description: ''
  name: firstSeen
  type: object
- description: ''
  name: lastSeen
  type: object
- description: ''
  name: targets
  type: object
- description: ''
  name: ttps
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-atig-data-schema.json
slug: inspector-atig-data
source_filename: inspector-atig-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-atig-data-schema.json\",\n  \"title\": \"AtigData\",\n  \"description\": \"The Amazon Web Services Threat Intel Group (ATIG) details for a specific vulnerability.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"firstSeen\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FirstSeen\"\n        },\n        {\n          \"description\": \"The date and time this vulnerability was first observed.\"\n        }\n      ]\n    },\n    \"lastSeen\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastSeen\"\n        },\n        {\n          \"description\": \"The date and time this vulnerability was last observed.\"\n        }\n      ]\n    },\n    \"targets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Targets\"\
  \n        },\n        {\n          \"description\": \"The commercial sectors this vulnerability targets.\"\n        }\n      ]\n    },\n    \"ttps\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ttps\"\n        },\n        {\n          \"description\": \"The <a href=\\\"https://attack.mitre.org/\\\">MITRE ATT&amp;CK</a> tactics, techniques, and procedures (TTPs) associated with vulnerability.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-atig-data-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: AtigData
---
