---
description: An object that contains the counts of aggregated finding per severity.
layout: schema
name: SeverityCounts
properties_list:
- description: ''
  name: all
  type: object
- description: ''
  name: critical
  type: object
- description: ''
  name: high
  type: object
- description: ''
  name: medium
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-severity-counts-schema.json
slug: inspector-severity-counts
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-severity-counts-schema.json\",\n  \"title\": \"SeverityCounts\",\n  \"description\": \"An object that contains the counts of aggregated finding per severity.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"all\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The total count of findings from all severities.\"\n        }\n      ]\n    },\n    \"critical\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The total count of critical severity findings.\"\n        }\n      ]\n    },\n    \"high\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n        \
  \  \"description\": \"The total count of high severity findings.\"\n        }\n      ]\n    },\n    \"medium\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The total count of medium severity findings.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-severity-counts-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: SeverityCounts
---
