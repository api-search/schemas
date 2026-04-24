---
description: An access request for a privileged account.
layout: schema
name: Request
properties_list:
- description: Unique identifier of the request.
  name: RequestID
  type: integer
- description: Current status of the request.
  name: Status
  type: string
- description: Type of access requested.
  name: AccessType
  type: string
- description: Name of the privileged account.
  name: AccountName
  type: string
- description: ID of the managed account.
  name: AccountID
  type: integer
- description: Name of the target system.
  name: SystemName
  type: string
- description: ID of the managed system.
  name: SystemID
  type: integer
- description: When the approved request expires.
  name: ExpiresDate
  type: string
- description: Requested duration in minutes.
  name: RequestedDurationMinutes
  type: integer
- description: Reason provided for the access request.
  name: Reason
  type: string
- description: When the request was created.
  name: RequestDate
  type: string
provider_name: BeyondTrust
provider_slug: beyondtrust
schema_file: json-schema/beyondtrust-request-schema.json
slug: beyondtrust-request
tags:
- Access
- Access Management
- Compliance
- Credentials
- Privileged Access
- Security
- Secrets
- Zero Trust
title: Request
---
