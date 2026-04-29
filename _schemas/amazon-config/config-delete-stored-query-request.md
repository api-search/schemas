---
description: DeleteStoredQueryRequest schema
layout: schema
name: DeleteStoredQueryRequest
properties_list:
- description: ''
  name: QueryName
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-delete-stored-query-request-schema.json
slug: config-delete-stored-query-request
source_filename: config-delete-stored-query-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-delete-stored-query-request-schema.json\",\n  \"title\": \"DeleteStoredQueryRequest\",\n  \"description\": \"DeleteStoredQueryRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"QueryName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueryName\"\n        },\n        {\n          \"description\": \"The name of the query that you want to delete.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"QueryName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-delete-stored-query-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DeleteStoredQueryRequest
---
