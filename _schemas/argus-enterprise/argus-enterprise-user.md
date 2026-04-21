---
description: User schema from ARGUS Enterprise API
layout: schema
name: User
properties_list:
- description: Unique user identifier
  name: id
  type: string
- description: Username
  name: username
  type: string
- description: User email address
  name: email
  type: string
- description: First name
  name: firstName
  type: string
- description: Last name
  name: lastName
  type: string
- description: User role
  name: role
  type: string
- description: Last login timestamp
  name: lastLogin
  type: string
- description: Whether the user account is active
  name: active
  type: boolean
- description: ''
  name: createdAt
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-user-schema.json
slug: argus-enterprise-user
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: User
---
