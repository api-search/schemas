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
