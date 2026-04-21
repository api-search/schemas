---
description: Successful authentication response
layout: schema
name: LoginResponse
properties_list:
- description: Shiro session identifier
  name: sessionId
  type: string
- description: Authenticated principal name
  name: principal
  type: string
- description: Roles assigned to the user
  name: roles
  type: array
- description: Explicit permissions granted to the user
  name: permissions
  type: array
provider_name: Apache Shiro
provider_slug: apache-shiro
schema_file: json-schema/apache-shiro-login-response-schema.json
slug: apache-shiro-login-response
tags:
- Authentication
- Authorization
- Cryptography
- Java
- Security
- Apache
- Open Source
title: LoginResponse
---
