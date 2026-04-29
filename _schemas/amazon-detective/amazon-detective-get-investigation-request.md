---
description: Request to get investigation details
layout: schema
name: GetInvestigationRequest
properties_list:
- description: The ARN of the behavior graph.
  name: GraphArn
  type: string
- description: The investigation ID of the investigation report.
  name: InvestigationId
  type: string
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-get-investigation-request-schema.json
slug: amazon-detective-get-investigation-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-get-investigation-request-schema.json\",\n  \"title\": \"GetInvestigationRequest\",\n  \"description\": \"Request to get investigation details\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GraphArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the behavior graph.\",\n      \"example\": \"arn:aws:detective:us-east-1:123456789012:graph:abc123def456\"\n    },\n    \"InvestigationId\": {\n      \"type\": \"string\",\n      \"description\": \"The investigation ID of the investigation report.\",\n      \"example\": \"invest-abc123def456\"\n    }\n  },\n  \"required\": [\n    \"GraphArn\",\n    \"InvestigationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-get-investigation-request-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: GetInvestigationRequest
---
