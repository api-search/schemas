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
source_filename: apache-shiro-hash-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-shiro/refs/heads/main/json-schema/apache-shiro-hash-request-schema.json\",\n  \"title\": \"HashRequest\",\n  \"description\": \"Password hashing request\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"Plain text password to hash\"\n    },\n    \"algorithm\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"MD5\",\n        \"SHA-1\",\n        \"SHA-256\",\n        \"SHA-512\",\n        \"Argon2\",\n        \"bcrypt\"\n      ],\n      \"description\": \"Hash algorithm to use\"\n    },\n    \"iterations\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of hash iterations\"\n    }\n  },\n  \"required\": [\n    \"password\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-shiro/refs/heads/main/json-schema/apache-shiro-hash-request-schema.json
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
