---
description: Request body for submitting an approval action.
layout: schema
name: ApprovalActionRequest
properties_list:
- description: Task identifier.
  name: taskId
  type: string
- description: Action to take.
  name: action
  type: string
- description: User ID submitting the action.
  name: userId
  type: string
- description: Optional comment for the action.
  name: comment
  type: string
provider_name: Ariba Sourcing
provider_slug: ariba-sourcing
schema_file: json-schema/external-approval-api-approval-action-request-schema.json
slug: external-approval-api-approval-action-request
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
title: ApprovalActionRequest
---
