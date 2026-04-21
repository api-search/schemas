---
description: JWT or token-based authentication response
layout: schema
name: TokenResponse
properties_list:
- description: Authentication token
  name: token
  type: string
- description: Token type (e.g. Bearer)
  name: tokenType
  type: string
- description: Token expiry in seconds
  name: expiresIn
  type: integer
- description: Authenticated principal
  name: principal
  type: string
provider_name: Apache Shiro
provider_slug: apache-shiro
schema_file: json-schema/apache-shiro-token-response-schema.json
slug: apache-shiro-token-response
tags:
- Authentication
- Authorization
- Cryptography
- Java
- Security
- Apache
- Open Source
title: TokenResponse
---
