---
description: An approval request entry.
layout: schema
name: ApprovalRequest
properties_list:
- description: List of approvers.
  name: approvers
  type: array
provider_name: Ariba Sourcing
provider_slug: ariba-sourcing
schema_file: json-schema/external-approval-api-approval-request-schema.json
slug: external-approval-api-approval-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/json-schema/external-approval-api-approval-request-schema.json\",\n  \"title\": \"ApprovalRequest\",\n  \"description\": \"An approval request entry.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"approvers\": {\n      \"type\": \"array\",\n      \"description\": \"List of approvers.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Approver\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/json-schema/external-approval-api-approval-request-schema.json
tags:
- Approvals
- Auctions
- B2B
- Contracts
- Procurement
- RFx
- SAP
- Sourcing
- Supplier Management
- Supply Chain
title: ApprovalRequest
---
