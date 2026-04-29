---
description: Describes a resource tag
layout: schema
name: Tag
properties_list:
- description: The key of the tag
  name: key
  type: string
- description: The value of the tag
  name: value
  type: string
provider_name: Amazon RDS
provider_slug: amazon-rds
schema_file: json-schema/amazon-rds-openapi-tag-schema.json
slug: amazon-rds-openapi-tag
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rds/refs/heads/main/json-schema/amazon-rds-openapi-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"Describes a resource tag\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The key of the tag\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The value of the tag\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rds/refs/heads/main/json-schema/amazon-rds-openapi-tag-schema.json
tags:
- AWS
- Cloud Databases
- Database Service
- DBaaS
- Managed Databases
- Relational Databases
title: Tag
---
