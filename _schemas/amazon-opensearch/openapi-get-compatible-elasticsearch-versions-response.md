---
description: Container for response returned by <code> <a>GetCompatibleElasticsearchVersions</a> </code> operation.
layout: schema
name: GetCompatibleElasticsearchVersionsResponse
properties_list:
- description: ''
  name: CompatibleElasticsearchVersions
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-get-compatible-elasticsearch-versions-response-schema.json
slug: openapi-get-compatible-elasticsearch-versions-response
source_filename: openapi-get-compatible-elasticsearch-versions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-get-compatible-elasticsearch-versions-response-schema.json\",\n  \"title\": \"GetCompatibleElasticsearchVersionsResponse\",\n  \"description\": \" Container for response returned by <code> <a>GetCompatibleElasticsearchVersions</a> </code> operation. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CompatibleElasticsearchVersions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CompatibleElasticsearchVersionsList\"\n        },\n        {\n          \"description\": \" A map of compatible Elasticsearch versions returned as part of the <code> <a>GetCompatibleElasticsearchVersions</a> </code> operation. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-get-compatible-elasticsearch-versions-response-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: GetCompatibleElasticsearchVersionsResponse
---
