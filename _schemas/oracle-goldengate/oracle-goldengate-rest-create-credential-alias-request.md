---
description: ''
layout: schema
name: CreateCredentialAliasRequest
properties_list:
- description: Database user ID including connect string
  name: userid
  type: string
- description: Password for the user
  name: password
  type: string
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-create-credential-alias-request-schema.json
slug: oracle-goldengate-rest-create-credential-alias-request
source_filename: oracle-goldengate-rest-create-credential-alias-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateCredentialAliasRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userid\": {\n      \"type\": \"string\",\n      \"description\": \"Database user ID including connect string\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"Password for the user\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-create-credential-alias-request-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: CreateCredentialAliasRequest
---
