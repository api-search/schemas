---
description: The Common Vulnerability Scoring System (CVSS) version 2 details for the vulnerability.
layout: schema
name: Cvss2
properties_list:
- description: ''
  name: baseScore
  type: object
- description: ''
  name: scoringVector
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-cvss2-schema.json
slug: inspector-cvss2
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-cvss2-schema.json\",\n  \"title\": \"Cvss2\",\n  \"description\": \"The Common Vulnerability Scoring System (CVSS) version 2 details for the vulnerability.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"baseScore\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Cvss2BaseScore\"\n        },\n        {\n          \"description\": \"The CVSS v2 base score for the vulnerability.\"\n        }\n      ]\n    },\n    \"scoringVector\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Cvss2ScoringVector\"\n        },\n        {\n          \"description\": \"The scoring vector associated with the CVSS v2 score.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-cvss2-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: Cvss2
---
