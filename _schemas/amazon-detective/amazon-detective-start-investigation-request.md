---
description: Request to start an investigation
layout: schema
name: StartInvestigationRequest
properties_list:
- description: The ARN of the behavior graph.
  name: GraphArn
  type: string
- description: The unique Amazon Resource Name (ARN) of the IAM user and IAM role.
  name: EntityArn
  type: string
- description: The data and time when the investigation began.
  name: ScopeStartTime
  type: string
- description: The data and time when the investigation ended.
  name: ScopeEndTime
  type: string
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-start-investigation-request-schema.json
slug: amazon-detective-start-investigation-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-start-investigation-request-schema.json\",\n  \"title\": \"StartInvestigationRequest\",\n  \"description\": \"Request to start an investigation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GraphArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the behavior graph.\",\n      \"example\": \"arn:aws:detective:us-east-1:123456789012:graph:abc123def456\"\n    },\n    \"EntityArn\": {\n      \"type\": \"string\",\n      \"description\": \"The unique Amazon Resource Name (ARN) of the IAM user and IAM role.\",\n      \"example\": \"arn:aws:iam::123456789012:user/jsmith\"\n    },\n    \"ScopeStartTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The data and time when the investigation began.\",\n      \"example\"\
  : \"2025-01-01T00:00:00Z\"\n    },\n    \"ScopeEndTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The data and time when the investigation ended.\",\n      \"example\": \"2025-01-15T23:59:59Z\"\n    }\n  },\n  \"required\": [\n    \"GraphArn\",\n    \"EntityArn\",\n    \"ScopeStartTime\",\n    \"ScopeEndTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-start-investigation-request-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: StartInvestigationRequest
---
