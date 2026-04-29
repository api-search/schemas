---
description: ListCheckSummariesInput schema from AWS Well-Architected Tool API
layout: schema
name: ListCheckSummariesInput
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: LensArn
  type: object
- description: ''
  name: PillarId
  type: object
- description: ''
  name: QuestionId
  type: object
- description: ''
  name: ChoiceId
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-list-check-summaries-input-schema.json
slug: well-architected-tool-list-check-summaries-input
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"LensArn\",\n    \"PillarId\",\n    \"QuestionId\",\n    \"ChoiceId\"\n  ],\n  \"title\": \"ListCheckSummariesInput\",\n  \"properties\": {\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/NextToken\"\n    },\n    \"MaxResults\": {\n      \"$ref\": \"#/components/schemas/MaxResults\"\n    },\n    \"LensArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LensArn\"\n        },\n        {\n          \"description\": \"Well-Architected Lens ARN.\"\n        }\n      ]\n    },\n    \"PillarId\": {\n      \"$ref\": \"#/components/schemas/PillarId\"\n    },\n    \"QuestionId\": {\n      \"$ref\": \"#/components/schemas/QuestionId\"\n    },\n    \"ChoiceId\": {\n      \"$ref\": \"#/components/schemas/ChoiceId\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-list-check-summaries-input-schema.json\"\
  ,\n  \"description\": \"ListCheckSummariesInput schema from AWS Well-Architected Tool API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-list-check-summaries-input-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ListCheckSummariesInput
---
