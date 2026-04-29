---
description: PutStoredQueryResponse schema
layout: schema
name: PutStoredQueryResponse
properties_list:
- description: ''
  name: QueryArn
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-put-stored-query-response-schema.json
slug: config-put-stored-query-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-stored-query-response-schema.json\",\n  \"title\": \"PutStoredQueryResponse\",\n  \"description\": \"PutStoredQueryResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"QueryArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueryArn\"\n        },\n        {\n          \"description\": \"Amazon Resource Name (ARN) of the query. For example, arn:partition:service:region:account-id:resource-type/resource-name/resource-id.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-stored-query-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: PutStoredQueryResponse
---
