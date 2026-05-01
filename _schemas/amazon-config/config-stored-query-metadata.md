---
description: Returns details of a specific query.
layout: schema
name: StoredQueryMetadata
properties_list:
- description: ''
  name: QueryId
  type: object
- description: ''
  name: QueryArn
  type: object
- description: ''
  name: QueryName
  type: object
- description: ''
  name: Description
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-stored-query-metadata-schema.json
slug: config-stored-query-metadata
source_filename: config-stored-query-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-stored-query-metadata-schema.json\",\n  \"title\": \"StoredQueryMetadata\",\n  \"description\": \"Returns details of a specific query. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"QueryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueryId\"\n        },\n        {\n          \"description\": \"The ID of the query. \"\n        }\n      ]\n    },\n    \"QueryArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueryArn\"\n        },\n        {\n          \"description\": \"Amazon Resource Name (ARN) of the query. For example, arn:partition:service:region:account-id:resource-type/resource-name/resource-id.\"\n        }\n      ]\n    },\n    \"QueryName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueryName\"\
  \n        },\n        {\n          \"description\": \"The name of the query.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueryDescription\"\n        },\n        {\n          \"description\": \"A unique description for the query.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"QueryId\",\n    \"QueryArn\",\n    \"QueryName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-stored-query-metadata-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: StoredQueryMetadata
---
