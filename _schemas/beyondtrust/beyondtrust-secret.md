---
description: A secret stored in BeyondTrust Secrets Safe.
layout: schema
name: Secret
properties_list:
- description: Unique identifier of the secret.
  name: id
  type: string
- description: Title or name of the secret.
  name: title
  type: string
- description: Description of the secret.
  name: description
  type: string
- description: Type of secret.
  name: type
  type: string
- description: Folder organizing this secret.
  name: folderName
  type: string
- description: When the secret was created.
  name: created
  type: string
- description: When the secret was last modified.
  name: lastModified
  type: string
provider_name: BeyondTrust
provider_slug: beyondtrust
schema_file: json-schema/beyondtrust-secret-schema.json
slug: beyondtrust-secret
tags:
- Access
- Access Management
- Compliance
- Credentials
- Privileged Access
- Security
- Secrets
- Zero Trust
title: Secret
---
