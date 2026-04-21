---
description: Result of permission check
layout: schema
name: PermissionCheckResult
properties_list:
- description: Checked permission string
  name: permission
  type: string
- description: Whether the subject has the permission
  name: permitted
  type: boolean
- description: Subject being checked
  name: principal
  type: string
provider_name: Apache Shiro
provider_slug: apache-shiro
schema_file: json-schema/apache-shiro-permission-check-result-schema.json
slug: apache-shiro-permission-check-result
tags:
- Authentication
- Authorization
- Cryptography
- Java
- Security
- Apache
- Open Source
title: PermissionCheckResult
---
