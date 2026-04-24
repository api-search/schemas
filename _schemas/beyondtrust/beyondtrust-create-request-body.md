---
description: Request body for creating an access request.
layout: schema
name: CreateRequestBody
properties_list:
- description: ID of the managed system.
  name: SystemID
  type: integer
- description: ID of the managed account.
  name: AccountID
  type: integer
- description: Requested access duration in minutes.
  name: DurationMinutes
  type: integer
- description: Business justification for the access request.
  name: Reason
  type: string
- description: Type of access requested.
  name: AccessType
  type: string
provider_name: BeyondTrust
provider_slug: beyondtrust
schema_file: json-schema/beyondtrust-create-request-body-schema.json
slug: beyondtrust-create-request-body
tags:
- Access
- Access Management
- Compliance
- Credentials
- Privileged Access
- Security
- Secrets
- Zero Trust
title: CreateRequestBody
---
