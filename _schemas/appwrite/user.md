---
description: An Appwrite user account with authentication credentials
layout: schema
name: User
properties_list:
- description: Unique user identifier
  name: $id
  type: string
- description: User display name
  name: name
  type: string
- description: User email address
  name: email
  type: string
- description: User phone number
  name: phone
  type: string
- description: Whether email is verified
  name: emailVerification
  type: boolean
- description: Whether phone is verified
  name: phoneVerification
  type: boolean
- description: User account status (active/disabled)
  name: status
  type: boolean
- description: Account creation timestamp
  name: createdAt
  type: string
- description: Last update timestamp
  name: updatedAt
  type: string
- description: User labels for RBAC
  name: labels
  type: array
provider_name: Appwrite
provider_slug: appwrite
schema_file: json-schema/user-schema.json
slug: user
tags:
- Applications
- Backends
- Mobile
- Open Source
title: User
---
