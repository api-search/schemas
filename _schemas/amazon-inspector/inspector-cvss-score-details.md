---
description: Information about the CVSS score.
layout: schema
name: CvssScoreDetails
properties_list:
- description: ''
  name: adjustments
  type: object
- description: ''
  name: cvssSource
  type: object
- description: ''
  name: score
  type: object
- description: ''
  name: scoreSource
  type: object
- description: ''
  name: scoringVector
  type: object
- description: ''
  name: version
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-cvss-score-details-schema.json
slug: inspector-cvss-score-details
source_filename: inspector-cvss-score-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-cvss-score-details-schema.json\",\n  \"title\": \"CvssScoreDetails\",\n  \"description\": \"Information about the CVSS score.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"adjustments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CvssScoreAdjustmentList\"\n        },\n        {\n          \"description\": \"An object that contains details about adjustment Amazon Inspector made to the CVSS score.\"\n        }\n      ]\n    },\n    \"cvssSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The source of the CVSS data.\"\n        }\n      ]\n    },\n    \"score\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n\
  \        },\n        {\n          \"description\": \"The CVSS score.\"\n        }\n      ]\n    },\n    \"scoreSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The source for the CVSS score.\"\n        }\n      ]\n    },\n    \"scoringVector\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The vector for the CVSS score.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The CVSS version used in scoring.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"score\",\n    \"scoreSource\",\n    \"scoringVector\",\n    \"version\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-cvss-score-details-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: CvssScoreDetails
---
