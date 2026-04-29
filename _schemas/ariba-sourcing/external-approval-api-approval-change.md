---
description: An approval task state change record.
layout: schema
name: ApprovalChange
properties_list:
- description: Sequence ID of the change for pagination.
  name: changeSequenceId
  type: string
- description: Task identifier.
  name: taskId
  type: string
- description: Type of document being approved.
  name: documentType
  type: string
- description: Document identifier.
  name: documentId
  type: string
- description: Current task status.
  name: status
  type: string
- description: Full URL to view the approvable in the SAP Ariba UI.
  name: fullURL
  type: string
provider_name: Ariba Sourcing
provider_slug: ariba-sourcing
schema_file: json-schema/external-approval-api-approval-change-schema.json
slug: external-approval-api-approval-change
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/json-schema/external-approval-api-approval-change-schema.json\",\n  \"title\": \"ApprovalChange\",\n  \"description\": \"An approval task state change record.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"changeSequenceId\": {\n      \"type\": \"string\",\n      \"description\": \"Sequence ID of the change for pagination.\",\n      \"example\": \"12345\"\n    },\n    \"taskId\": {\n      \"type\": \"string\",\n      \"description\": \"Task identifier.\",\n      \"example\": \"TASK-500123\"\n    },\n    \"documentType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of document being approved.\",\n      \"example\": \"RFXDocument\"\n    },\n    \"documentId\": {\n      \"type\": \"string\",\n      \"description\": \"Document identifier.\",\n      \"example\": \"DOC-001234\"\n    },\n    \"\
  status\": {\n      \"type\": \"string\",\n      \"description\": \"Current task status.\",\n      \"example\": \"submitted\"\n    },\n    \"fullURL\": {\n      \"type\": \"string\",\n      \"description\": \"Full URL to view the approvable in the SAP Ariba UI.\",\n      \"example\": \"https://mycompany-T.sourcing.ariba.com/Sourcing/main/ad/taskWorkspace\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/json-schema/external-approval-api-approval-change-schema.json
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
title: ApprovalChange
---
