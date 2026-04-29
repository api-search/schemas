---
description: Response from listing indicators
layout: schema
name: ListIndicatorsResponse
properties_list:
- description: The ARN of the behavior graph.
  name: GraphArn
  type: string
- description: The investigation ID of the investigation report.
  name: InvestigationId
  type: string
- description: List if there are more results available.
  name: NextToken
  type: string
- description: Lists the indicators of compromise.
  name: Indicators
  type: array
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-list-indicators-response-schema.json
slug: amazon-detective-list-indicators-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-list-indicators-response-schema.json\",\n  \"title\": \"ListIndicatorsResponse\",\n  \"description\": \"Response from listing indicators\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GraphArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the behavior graph.\",\n      \"example\": \"arn:aws:detective:us-east-1:123456789012:graph:abc123def456\"\n    },\n    \"InvestigationId\": {\n      \"type\": \"string\",\n      \"description\": \"The investigation ID of the investigation report.\",\n      \"example\": \"invest-abc123def456\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"List if there are more results available.\"\n    },\n    \"Indicators\": {\n      \"type\": \"array\",\n      \"description\": \"Lists the indicators\
  \ of compromise.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Indicator\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-list-indicators-response-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: ListIndicatorsResponse
---
