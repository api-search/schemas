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
source_filename: apache-shiro-hash-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-shiro/refs/heads/main/json-schema/apache-shiro-hash-result-schema.json\",\n  \"title\": \"HashResult\",\n  \"description\": \"Password hash result\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"hash\": {\n      \"type\": \"string\",\n      \"description\": \"Hashed password value\"\n    },\n    \"salt\": {\n      \"type\": \"string\",\n      \"description\": \"Salt used for hashing\"\n    },\n    \"algorithm\": {\n      \"type\": \"string\",\n      \"description\": \"Algorithm used\"\n    },\n    \"iterations\": {\n      \"type\": \"integer\",\n      \"description\": \"Iterations applied\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-shiro/refs/heads/main/json-schema/apache-shiro-hash-result-schema.json
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
