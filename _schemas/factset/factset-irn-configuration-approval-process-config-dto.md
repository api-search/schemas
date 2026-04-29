---
description: ''
layout: schema
name: ApprovalProcessConfigDto
properties_list:
- description: ''
  name: approvalLevels
  type: array
- description: ''
  name: viewerIds
  type: array
- description: ''
  name: shouldSendEmailAlertsWhenSubmittedForApproval
  type: boolean
- description: ''
  name: shouldSendEmailAlertsWhenApproved
  type: boolean
- description: ''
  name: shouldSendEmailAlertsWhenDenied
  type: boolean
- description: ''
  name: shouldSendEmailAlertsToAuthor
  type: boolean
- description: ''
  name: shouldSendEmailAlertsToApprovers
  type: boolean
- description: ''
  name: shouldSendEmailAlertsToViewers
  type: boolean
- description: ''
  name: canAuthorSelfApprove
  type: boolean
- description: ''
  name: canAuthorEditPending
  type: boolean
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-irn-configuration-approval-process-config-dto-schema.json
slug: factset-irn-configuration-approval-process-config-dto
source_filename: factset-irn-configuration-approval-process-config-dto-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApprovalProcessConfigDto\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"approvalLevels\": {\n      \"type\": \"array\"\n    },\n    \"viewerIds\": {\n      \"type\": \"array\"\n    },\n    \"shouldSendEmailAlertsWhenSubmittedForApproval\": {\n      \"type\": \"boolean\"\n    },\n    \"shouldSendEmailAlertsWhenApproved\": {\n      \"type\": \"boolean\"\n    },\n    \"shouldSendEmailAlertsWhenDenied\": {\n      \"type\": \"boolean\"\n    },\n    \"shouldSendEmailAlertsToAuthor\": {\n      \"type\": \"boolean\"\n    },\n    \"shouldSendEmailAlertsToApprovers\": {\n      \"type\": \"boolean\"\n    },\n    \"shouldSendEmailAlertsToViewers\": {\n      \"type\": \"boolean\"\n    },\n    \"canAuthorSelfApprove\": {\n      \"type\": \"boolean\"\n    },\n    \"canAuthorEditPending\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-irn-configuration-approval-process-config-dto-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: ApprovalProcessConfigDto
---
