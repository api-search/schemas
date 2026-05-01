---
description: The CVSS score for a finding.
layout: schema
name: CvssScore
properties_list:
- description: ''
  name: baseScore
  type: object
- description: ''
  name: scoringVector
  type: object
- description: ''
  name: source
  type: object
- description: ''
  name: version
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-cvss-score-schema.json
slug: inspector-cvss-score
source_filename: inspector-cvss-score-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-cvss-score-schema.json\",\n  \"title\": \"CvssScore\",\n  \"description\": \"The CVSS score for a finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"baseScore\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"The base CVSS score used for the finding.\"\n        }\n      ]\n    },\n    \"scoringVector\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The vector string of the CVSS score.\"\n        }\n      ]\n    },\n    \"source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The source of\
  \ the CVSS score.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The version of CVSS used for the score.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"baseScore\",\n    \"scoringVector\",\n    \"source\",\n    \"version\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-cvss-score-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: CvssScore
---
