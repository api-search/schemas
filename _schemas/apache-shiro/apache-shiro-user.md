---
description: User account
layout: schema
name: User
properties_list:
- description: User identifier
  name: id
  type: string
- description: Username
  name: username
  type: string
- description: Email address
  name: email
  type: string
- description: Assigned roles
  name: roles
  type: array
- description: Whether the account is locked
  name: locked
  type: boolean
provider_name: Apache Shiro
provider_slug: apache-shiro
schema_file: json-schema/apache-shiro-user-schema.json
slug: apache-shiro-user
tags:
- Authentication
- Authorization
- Cryptography
- Java
- Security
- Apache
- Open Source
title: User
---
