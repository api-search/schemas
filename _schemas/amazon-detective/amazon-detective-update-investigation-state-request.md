---
description: Request to update the state of an investigation
layout: schema
name: UpdateInvestigationStateRequest
properties_list:
- description: The ARN of the behavior graph.
  name: GraphArn
  type: string
- description: The investigation ID of the investigation report.
  name: InvestigationId
  type: string
- description: The current state of the investigation. An archived investigation indicates you have completed reviewing the investigation.
  name: State
  type: string
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-update-investigation-state-request-schema.json
slug: amazon-detective-update-investigation-state-request
source_filename: amazon-detective-update-investigation-state-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-update-investigation-state-request-schema.json\",\n  \"title\": \"UpdateInvestigationStateRequest\",\n  \"description\": \"Request to update the state of an investigation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GraphArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the behavior graph.\",\n      \"example\": \"arn:aws:detective:us-east-1:123456789012:graph:abc123def456\"\n    },\n    \"InvestigationId\": {\n      \"type\": \"string\",\n      \"description\": \"The investigation ID of the investigation report.\",\n      \"example\": \"invest-abc123def456\"\n    },\n    \"State\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the investigation. An archived investigation indicates you have completed reviewing the investigation.\"\
  ,\n      \"enum\": [\n        \"ACTIVE\",\n        \"ARCHIVED\"\n      ],\n      \"example\": \"ARCHIVED\"\n    }\n  },\n  \"required\": [\n    \"GraphArn\",\n    \"InvestigationId\",\n    \"State\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-update-investigation-state-request-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: UpdateInvestigationStateRequest
---
