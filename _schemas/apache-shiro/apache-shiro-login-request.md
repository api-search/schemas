---
description: User login credentials
layout: schema
name: LoginRequest
properties_list:
- description: Username or email
  name: username
  type: string
- description: User password
  name: password
  type: string
- description: Whether to set remember-me cookie
  name: rememberMe
  type: boolean
provider_name: Apache Shiro
provider_slug: apache-shiro
schema_file: json-schema/apache-shiro-login-request-schema.json
slug: apache-shiro-login-request
tags:
- Authentication
- Authorization
- Cryptography
- Java
- Security
- Apache
- Open Source
title: LoginRequest
---
