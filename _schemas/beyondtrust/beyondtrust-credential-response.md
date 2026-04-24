---
description: Credentials retrieved for an approved access request.
layout: schema
name: CredentialResponse
properties_list:
- description: The retrieved password. Only present for password-based accounts.
  name: Password
  type: string
- description: SSH private key. Only present for SSH key-based accounts.
  name: PrivateKey
  type: string
provider_name: BeyondTrust
provider_slug: beyondtrust
schema_file: json-schema/beyondtrust-credential-response-schema.json
slug: beyondtrust-credential-response
tags:
- Access
- Access Management
- Compliance
- Credentials
- Privileged Access
- Security
- Secrets
- Zero Trust
title: CredentialResponse
---
