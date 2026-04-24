---
description: A secret including its sensitive value.
layout: schema
name: SecretWithValue
properties_list:
- description: Unique identifier.
  name: id
  type: string
- description: Secret title.
  name: title
  type: string
- description: Secret type.
  name: type
  type: string
- description: Password value (for Password type secrets).
  name: password
  type: string
- description: Text value (for Text type secrets).
  name: text
  type: string
- description: Folder name.
  name: folderName
  type: string
- description: Creation timestamp.
  name: created
  type: string
provider_name: BeyondTrust
provider_slug: beyondtrust
schema_file: json-schema/beyondtrust-secret-with-value-schema.json
slug: beyondtrust-secret-with-value
tags:
- Access
- Access Management
- Compliance
- Credentials
- Privileged Access
- Security
- Secrets
- Zero Trust
title: SecretWithValue
---
