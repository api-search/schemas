---
description: Response containing group members.
layout: schema
name: GroupMembersResponse
properties_list:
- description: Group identifier.
  name: groupId
  type: string
- description: List of group member users.
  name: members
  type: array
provider_name: Ariba Sourcing
provider_slug: ariba-sourcing
schema_file: json-schema/external-approval-api-group-members-response-schema.json
slug: external-approval-api-group-members-response
source_filename: external-approval-api-group-members-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/json-schema/external-approval-api-group-members-response-schema.json\",\n  \"title\": \"GroupMembersResponse\",\n  \"description\": \"Response containing group members.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"groupId\": {\n      \"type\": \"string\",\n      \"description\": \"Group identifier.\",\n      \"example\": \"GROUP-001\"\n    },\n    \"members\": {\n      \"type\": \"array\",\n      \"description\": \"List of group member users.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/GroupMember\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/json-schema/external-approval-api-group-members-response-schema.json
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
title: GroupMembersResponse
---
