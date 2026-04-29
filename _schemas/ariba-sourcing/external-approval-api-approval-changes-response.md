---
description: Response containing changed approval tasks.
layout: schema
name: ApprovalChangesResponse
properties_list:
- description: List of approval task changes.
  name: changes
  type: array
provider_name: Ariba Sourcing
provider_slug: ariba-sourcing
schema_file: json-schema/external-approval-api-approval-changes-response-schema.json
slug: external-approval-api-approval-changes-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/json-schema/external-approval-api-approval-changes-response-schema.json\",\n  \"title\": \"ApprovalChangesResponse\",\n  \"description\": \"Response containing changed approval tasks.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"changes\": {\n      \"type\": \"array\",\n      \"description\": \"List of approval task changes.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ApprovalChange\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/json-schema/external-approval-api-approval-changes-response-schema.json
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
title: ApprovalChangesResponse
---
