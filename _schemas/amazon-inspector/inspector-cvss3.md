---
description: The Common Vulnerability Scoring System (CVSS) version 3 details for the vulnerability.
layout: schema
name: Cvss3
properties_list:
- description: ''
  name: baseScore
  type: object
- description: ''
  name: scoringVector
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-cvss3-schema.json
slug: inspector-cvss3
source_filename: inspector-cvss3-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-cvss3-schema.json\",\n  \"title\": \"Cvss3\",\n  \"description\": \"The Common Vulnerability Scoring System (CVSS) version 3 details for the vulnerability.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"baseScore\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Cvss3BaseScore\"\n        },\n        {\n          \"description\": \"The CVSS v3 base score for the vulnerability.\"\n        }\n      ]\n    },\n    \"scoringVector\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Cvss3ScoringVector\"\n        },\n        {\n          \"description\": \"The scoring vector associated with the CVSS v3 score.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-cvss3-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: Cvss3
---
