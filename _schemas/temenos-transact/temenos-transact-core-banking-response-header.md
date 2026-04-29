---
description: Standard response header returned by all Transact API operations
layout: schema
name: ResponseHeader
properties_list:
- description: Unique identifier for the resource
  name: id
  type: string
- description: Status of the operation (success, error)
  name: status
  type: string
- description: Transaction lifecycle status
  name: transactionStatus
  type: string
- description: ''
  name: audit
  type: object
provider_name: Temenos Transact
provider_slug: temenos-transact
schema_file: json-schema/temenos-transact-core-banking-response-header-schema.json
slug: temenos-transact-core-banking-response-header
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResponseHeader\",\n  \"type\": \"object\",\n  \"description\": \"Standard response header returned by all Transact API operations\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the resource\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the operation (success, error)\"\n    },\n    \"transactionStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction lifecycle status\"\n    },\n    \"audit\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/json-schema/temenos-transact-core-banking-response-header-schema.json
tags:
- Banking
- Core Banking
- Digital Banking
- Enterprise
- Financial Services
- Fintech
title: ResponseHeader
---
