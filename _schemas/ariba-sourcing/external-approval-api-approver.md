---
description: An individual or group approver.
layout: schema
name: Approver
properties_list:
- description: User identifier.
  name: userId
  type: string
- description: Approver display name.
  name: name
  type: string
provider_name: Ariba Sourcing
provider_slug: ariba-sourcing
schema_file: json-schema/external-approval-api-approver-schema.json
slug: external-approval-api-approver
source_filename: external-approval-api-approver-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/json-schema/external-approval-api-approver-schema.json\",\n  \"title\": \"Approver\",\n  \"description\": \"An individual or group approver.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"User identifier.\",\n      \"example\": \"jsmith@example.com\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Approver display name.\",\n      \"example\": \"Jane Smith\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/json-schema/external-approval-api-approver-schema.json
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
title: Approver
---
