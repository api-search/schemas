---
description: Request body for creating a new secret.
layout: schema
name: CreateSecretRequest
properties_list:
- description: Title of the secret.
  name: title
  type: string
- description: Description of the secret.
  name: description
  type: string
- description: Type of secret.
  name: type
  type: string
- description: Password value (for Password type).
  name: password
  type: string
- description: Text value (for Text type).
  name: text
  type: string
- description: Folder to store the secret in.
  name: folderName
  type: string
provider_name: BeyondTrust
provider_slug: beyondtrust
schema_file: json-schema/beyondtrust-create-secret-request-schema.json
slug: beyondtrust-create-secret-request
tags:
- Access
- Access Management
- Compliance
- Credentials
- Privileged Access
- Security
- Secrets
- Zero Trust
title: CreateSecretRequest
---
