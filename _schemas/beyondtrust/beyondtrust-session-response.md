---
description: Authenticated user session details.
layout: schema
name: SessionResponse
properties_list:
- description: Internal user ID.
  name: UserId
  type: integer
- description: Email address of the authenticated user.
  name: EmailAddress
  type: string
- description: Username of the authenticated user.
  name: UserName
  type: string
- description: Display name of the authenticated user.
  name: Name
  type: string
provider_name: BeyondTrust
provider_slug: beyondtrust
schema_file: json-schema/beyondtrust-session-response-schema.json
slug: beyondtrust-session-response
tags:
- Access
- Access Management
- Compliance
- Credentials
- Privileged Access
- Security
- Secrets
- Zero Trust
title: SessionResponse
---
