---
description: Account schema from Amazon Organizations
layout: schema
name: Account
properties_list:
- description: ''
  name: Id
  type: string
- description: ''
  name: Arn
  type: string
- description: ''
  name: Email
  type: string
- description: ''
  name: Name
  type: string
- description: ''
  name: Status
  type: string
- description: ''
  name: JoinedMethod
  type: string
- description: ''
  name: JoinedTimestamp
  type: string
provider_name: Amazon Organizations
provider_slug: amazon-organizations
schema_file: json-schema/openapi-account-schema.json
slug: openapi-account
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-organizations/refs/heads/main/json-schema/openapi-account-schema.json\",\n  \"title\": \"Account\",\n  \"description\": \"Account schema from Amazon Organizations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\"\n    },\n    \"Arn\": {\n      \"type\": \"string\"\n    },\n    \"Email\": {\n      \"type\": \"string\"\n    },\n    \"Name\": {\n      \"type\": \"string\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"SUSPENDED\",\n        \"PENDING_CLOSURE\"\n      ]\n    },\n    \"JoinedMethod\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"INVITED\",\n        \"CREATED\"\n      ]\n    },\n    \"JoinedTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-organizations/refs/heads/main/json-schema/openapi-account-schema.json
tags:
- Account Management
- AWS
- Consolidated Billing
- Governance
- Multi-Account
- Organizations
- Policies
title: Account
---
