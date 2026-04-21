---
description: Password hashing request
layout: schema
name: HashRequest
properties_list:
- description: Plain text password to hash
  name: password
  type: string
- description: Hash algorithm to use
  name: algorithm
  type: string
- description: Number of hash iterations
  name: iterations
  type: integer
provider_name: Apache Shiro
provider_slug: apache-shiro
schema_file: json-schema/apache-shiro-hash-request-schema.json
slug: apache-shiro-hash-request
tags:
- Authentication
- Authorization
- Cryptography
- Java
- Security
- Apache
- Open Source
title: HashRequest
---
