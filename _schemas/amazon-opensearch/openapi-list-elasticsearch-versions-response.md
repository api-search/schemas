---
description: Container for the parameters for response received from <code> <a>ListElasticsearchVersions</a> </code> operation.
layout: schema
name: ListElasticsearchVersionsResponse
properties_list:
- description: ''
  name: ElasticsearchVersions
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-list-elasticsearch-versions-response-schema.json
slug: openapi-list-elasticsearch-versions-response
source_filename: openapi-list-elasticsearch-versions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-list-elasticsearch-versions-response-schema.json\",\n  \"title\": \"ListElasticsearchVersionsResponse\",\n  \"description\": \" Container for the parameters for response received from <code> <a>ListElasticsearchVersions</a> </code> operation. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ElasticsearchVersions\": {\n      \"$ref\": \"#/components/schemas/ElasticsearchVersionList\"\n    },\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/NextToken\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-list-elasticsearch-versions-response-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: ListElasticsearchVersionsResponse
---
