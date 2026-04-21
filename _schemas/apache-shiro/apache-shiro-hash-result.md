---
description: Password hash result
layout: schema
name: HashResult
properties_list:
- description: Hashed password value
  name: hash
  type: string
- description: Salt used for hashing
  name: salt
  type: string
- description: Algorithm used
  name: algorithm
  type: string
- description: Iterations applied
  name: iterations
  type: integer
provider_name: Apache Shiro
provider_slug: apache-shiro
schema_file: json-schema/apache-shiro-hash-result-schema.json
slug: apache-shiro-hash-result
tags:
- Authentication
- Authorization
- Cryptography
- Java
- Security
- Apache
- Open Source
title: HashResult
---
