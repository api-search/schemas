---
description: ListStoredQueriesResponse schema
layout: schema
name: ListStoredQueriesResponse
properties_list:
- description: ''
  name: StoredQueryMetadata
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-list-stored-queries-response-schema.json
slug: config-list-stored-queries-response
source_filename: config-list-stored-queries-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-list-stored-queries-response-schema.json\",\n  \"title\": \"ListStoredQueriesResponse\",\n  \"description\": \"ListStoredQueriesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StoredQueryMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StoredQueryMetadataList\"\n        },\n        {\n          \"description\": \"A list of <code>StoredQueryMetadata</code> objects.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"If the previous paginated request didn't return all of the remaining results, the response object's <code>NextToken</code> parameter value is set to a token. To retrieve the next set of results,\
  \ call this action again and assign that token to the request object's <code>NextToken</code> parameter. If there are no remaining results, the previous response object's <code>NextToken</code> parameter is set to <code>null</code>. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-list-stored-queries-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ListStoredQueriesResponse
---
