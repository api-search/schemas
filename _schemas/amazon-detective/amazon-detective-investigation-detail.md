---
description: Summary details of an investigation
layout: schema
name: InvestigationDetail
properties_list:
- description: The investigation ID of the investigation report.
  name: InvestigationId
  type: string
- description: The severity assigned to the investigation.
  name: Severity
  type: string
- description: The status based on the completion status of the investigation.
  name: Status
  type: string
- description: The current state of the investigation.
  name: State
  type: string
- description: The time stamp of the creation time of the investigation report.
  name: CreatedTime
  type: string
- description: The unique Amazon Resource Name (ARN) of the IAM user and IAM role.
  name: EntityArn
  type: string
- description: Type of entity. For example, IAM_ROLE or IAM_USER.
  name: EntityType
  type: string
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-investigation-detail-schema.json
slug: amazon-detective-investigation-detail
source_filename: amazon-detective-investigation-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-investigation-detail-schema.json\",\n  \"title\": \"InvestigationDetail\",\n  \"description\": \"Summary details of an investigation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InvestigationId\": {\n      \"type\": \"string\",\n      \"description\": \"The investigation ID of the investigation report.\",\n      \"example\": \"invest-abc123def456\"\n    },\n    \"Severity\": {\n      \"type\": \"string\",\n      \"description\": \"The severity assigned to the investigation.\",\n      \"enum\": [\n        \"INFORMATIONAL\",\n        \"LOW\",\n        \"MEDIUM\",\n        \"HIGH\",\n        \"CRITICAL\"\n      ],\n      \"example\": \"HIGH\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"The status based on the completion status of the investigation.\"\
  ,\n      \"enum\": [\n        \"RUNNING\",\n        \"FAILED\",\n        \"SUCCESSFUL\"\n      ],\n      \"example\": \"RUNNING\"\n    },\n    \"State\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the investigation.\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"ARCHIVED\"\n      ],\n      \"example\": \"ACTIVE\"\n    },\n    \"CreatedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time stamp of the creation time of the investigation report.\",\n      \"example\": \"2025-01-15T10:00:00Z\"\n    },\n    \"EntityArn\": {\n      \"type\": \"string\",\n      \"description\": \"The unique Amazon Resource Name (ARN) of the IAM user and IAM role.\",\n      \"example\": \"arn:aws:iam::123456789012:user/jsmith\"\n    },\n    \"EntityType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of entity. For example, IAM_ROLE or IAM_USER.\",\n      \"enum\": [\n        \"IAM_ROLE\",\n       \
  \ \"IAM_USER\"\n      ],\n      \"example\": \"IAM_ROLE\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-investigation-detail-schema.json
tags:
- Forensics
- Investigation
- Security
title: InvestigationDetail
---
