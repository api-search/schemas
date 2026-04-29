---
description: An approvable document or project.
layout: schema
name: ApprovableDocument
properties_list:
- description: Document identifier.
  name: id
  type: string
- description: Document type.
  name: type
  type: string
- description: Document title.
  name: title
  type: string
- description: Document status.
  name: status
  type: string
- description: SAP Ariba realm name.
  name: realm
  type: string
provider_name: Ariba Sourcing
provider_slug: ariba-sourcing
schema_file: json-schema/external-approval-api-approvable-document-schema.json
slug: external-approval-api-approvable-document
source_filename: external-approval-api-approvable-document-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/json-schema/external-approval-api-approvable-document-schema.json\",\n  \"title\": \"ApprovableDocument\",\n  \"description\": \"An approvable document or project.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Document identifier.\",\n      \"example\": \"WS500123\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Document type.\",\n      \"example\": \"Workspace\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Document title.\",\n      \"example\": \"Q1 2026 Office Supplies RFQ\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Document status.\",\n      \"example\": \"pending\"\n    },\n    \"realm\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"SAP Ariba realm name.\",\n      \"example\": \"mycompany-T\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/json-schema/external-approval-api-approvable-document-schema.json
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
title: ApprovableDocument
---
