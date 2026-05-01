---
description: PutStoredQueryRequest schema
layout: schema
name: PutStoredQueryRequest
properties_list:
- description: ''
  name: StoredQuery
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-put-stored-query-request-schema.json
slug: config-put-stored-query-request
source_filename: config-put-stored-query-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-stored-query-request-schema.json\",\n  \"title\": \"PutStoredQueryRequest\",\n  \"description\": \"PutStoredQueryRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StoredQuery\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StoredQuery\"\n        },\n        {\n          \"description\": \"<p>A list of <code>StoredQuery</code> objects. The mandatory fields are <code>QueryName</code> and <code>Expression</code>.</p> <note> <p>When you are creating a query, you must provide a query name and an expression. When you are updating a query, you must provide a query name but updating the description is optional.</p> </note>\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagsList\"\
  \n        },\n        {\n          \"description\": \"A list of <code>Tags</code> object.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"StoredQuery\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-stored-query-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: PutStoredQueryRequest
---
