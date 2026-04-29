---
description: Response from getting investigation details
layout: schema
name: GetInvestigationResponse
properties_list:
- description: The ARN of the behavior graph.
  name: GraphArn
  type: string
- description: The investigation ID of the investigation report.
  name: InvestigationId
  type: string
- description: The unique Amazon Resource Name (ARN) of the IAM user and IAM role.
  name: EntityArn
  type: string
- description: Type of entity. For example, IAM_ROLE or IAM_USER.
  name: EntityType
  type: string
- description: The creation time of the investigation report in UTC time stamp format.
  name: CreatedTime
  type: string
- description: The start date and time used to set the scope time within which you want Detective to investigate.
  name: ScopeStartTime
  type: string
- description: The end date and time used to set the scope time within which you want Detective to investigate.
  name: ScopeEndTime
  type: string
- description: The status based on the completion status of the investigation.
  name: Status
  type: string
- description: The severity assigned is based on the likelihood and impact of the indicators of compromise discovered in the investigation.
  name: Severity
  type: string
- description: The current state of the investigation. An archived investigation indicates you have completed reviewing the investigation.
  name: State
  type: string
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-get-investigation-response-schema.json
slug: amazon-detective-get-investigation-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-get-investigation-response-schema.json\",\n  \"title\": \"GetInvestigationResponse\",\n  \"description\": \"Response from getting investigation details\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GraphArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the behavior graph.\",\n      \"example\": \"arn:aws:detective:us-east-1:123456789012:graph:abc123def456\"\n    },\n    \"InvestigationId\": {\n      \"type\": \"string\",\n      \"description\": \"The investigation ID of the investigation report.\",\n      \"example\": \"invest-abc123def456\"\n    },\n    \"EntityArn\": {\n      \"type\": \"string\",\n      \"description\": \"The unique Amazon Resource Name (ARN) of the IAM user and IAM role.\",\n      \"example\": \"arn:aws:iam::123456789012:user/jsmith\"\
  \n    },\n    \"EntityType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of entity. For example, IAM_ROLE or IAM_USER.\",\n      \"enum\": [\n        \"IAM_ROLE\",\n        \"IAM_USER\"\n      ],\n      \"example\": \"IAM_ROLE\"\n    },\n    \"CreatedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The creation time of the investigation report in UTC time stamp format.\",\n      \"example\": \"2025-01-15T10:00:00Z\"\n    },\n    \"ScopeStartTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The start date and time used to set the scope time within which you want Detective to investigate.\",\n      \"example\": \"2025-01-01T00:00:00Z\"\n    },\n    \"ScopeEndTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The end date and time used to set the scope time within which you want Detective to investigate.\",\n      \"example\"\
  : \"2025-01-15T23:59:59Z\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"The status based on the completion status of the investigation.\",\n      \"enum\": [\n        \"RUNNING\",\n        \"FAILED\",\n        \"SUCCESSFUL\"\n      ],\n      \"example\": \"RUNNING\"\n    },\n    \"Severity\": {\n      \"type\": \"string\",\n      \"description\": \"The severity assigned is based on the likelihood and impact of the indicators of compromise discovered in the investigation.\",\n      \"enum\": [\n        \"INFORMATIONAL\",\n        \"LOW\",\n        \"MEDIUM\",\n        \"HIGH\",\n        \"CRITICAL\"\n      ],\n      \"example\": \"HIGH\"\n    },\n    \"State\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the investigation. An archived investigation indicates you have completed reviewing the investigation.\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"ARCHIVED\"\n      ],\n      \"example\": \"ACTIVE\"\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-get-investigation-response-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: GetInvestigationResponse
---
