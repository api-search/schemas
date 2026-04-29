---
description: GetStoredQueryResponse schema
layout: schema
name: GetStoredQueryResponse
properties_list:
- description: ''
  name: StoredQuery
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-get-stored-query-response-schema.json
slug: config-get-stored-query-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-stored-query-response-schema.json\",\n  \"title\": \"GetStoredQueryResponse\",\n  \"description\": \"GetStoredQueryResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StoredQuery\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StoredQuery\"\n        },\n        {\n          \"description\": \"Returns a <code>StoredQuery</code> object.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-stored-query-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: GetStoredQueryResponse
---
