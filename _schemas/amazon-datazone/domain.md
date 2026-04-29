---
description: A DataZone domain that serves as the organizational boundary for data catalog and governance.
layout: schema
name: Domain
properties_list:
- description: The unique identifier of the domain
  name: id
  type: string
- description: The ARN of the DataZone domain. This ARN uniquely identifies the domain.
  name: arn
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: portalUrl
  type: string
- description: ''
  name: createdAt
  type: string
provider_name: Amazon DataZone
provider_slug: amazon-datazone
schema_file: json-schema/domain-schema.json
slug: domain
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-datazone/json-schema/domain-schema.json\",\n  \"title\": \"Domain\",\n  \"description\": \"A DataZone domain that serves as the organizational boundary for data catalog and governance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the domain\"\n    },\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the DataZone domain. This ARN uniquely identifies the domain.\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"AVAILABLE\",\n        \"CREATING\",\n        \"DELETED\"\n      ]\n    },\n    \"portalUrl\": {\n      \"type\": \"string\"\n    },\n    \"createdAt\": {\n      \"type\":\
  \ \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-datazone/refs/heads/main/json-schema/domain-schema.json
tags:
- AWS
- Data Catalog
- Data Governance
- Data Management
- Data Sharing
- Analytics
title: Domain
---
