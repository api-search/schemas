---
description: Response containing pending approval tasks.
layout: schema
name: PendingApprovablesResponse
properties_list:
- description: List of pending approval tasks.
  name: tasks
  type: array
provider_name: Ariba Sourcing
provider_slug: ariba-sourcing
schema_file: json-schema/external-approval-api-pending-approvables-response-schema.json
slug: external-approval-api-pending-approvables-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/json-schema/external-approval-api-pending-approvables-response-schema.json\",\n  \"title\": \"PendingApprovablesResponse\",\n  \"description\": \"Response containing pending approval tasks.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tasks\": {\n      \"type\": \"array\",\n      \"description\": \"List of pending approval tasks.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PendingApprovalTask\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/json-schema/external-approval-api-pending-approvables-response-schema.json
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
title: PendingApprovablesResponse
---
