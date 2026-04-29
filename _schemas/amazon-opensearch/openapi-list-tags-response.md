---
description: The result of a <code>ListTags</code> operation. Contains tags for all requested Elasticsearch domains.
layout: schema
name: ListTagsResponse
properties_list:
- description: ''
  name: TagList
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-list-tags-response-schema.json
slug: openapi-list-tags-response
source_filename: openapi-list-tags-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-list-tags-response-schema.json\",\n  \"title\": \"ListTagsResponse\",\n  \"description\": \"The result of a <code>ListTags</code> operation. Contains tags for all requested Elasticsearch domains.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TagList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \" List of <code>Tag</code> for the requested Elasticsearch domain.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-list-tags-response-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: ListTagsResponse
---
