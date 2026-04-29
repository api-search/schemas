---
description: ''
layout: schema
name: Fix
properties_list:
- description: Fix identifier
  name: id
  type: string
- description: Fix name
  name: name
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: description
  type: string
- description: CVEs resolved by this fix
  name: resolvedCVEs
  type: array
- description: WebSphere versions this fix applies to
  name: applicableVersions
  type: array
- description: ''
  name: downloadURL
  type: string
- description: ''
  name: releaseDate
  type: string
- description: Fix size in bytes
  name: size
  type: integer
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-automation-rest-fix-schema.json
slug: websphere-automation-rest-fix
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Fix\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Fix identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Fix name\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"resolvedCVEs\": {\n      \"type\": \"array\",\n      \"description\": \"CVEs resolved by this fix\"\n    },\n    \"applicableVersions\": {\n      \"type\": \"array\",\n      \"description\": \"WebSphere versions this fix applies to\"\n    },\n    \"downloadURL\": {\n      \"type\": \"string\"\n    },\n    \"releaseDate\": {\n      \"type\": \"string\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"Fix size in bytes\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-automation-rest-fix-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: Fix
---
