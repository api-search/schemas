---
description: Container for the parameters to the <code><a>RemoveTags</a></code> operation. Specify the <code>ARN</code> for the Elasticsearch domain from which you want to remove the specified <code>TagKey</code>.
layout: schema
name: RemoveTagsRequest
properties_list:
- description: ''
  name: ARN
  type: object
- description: ''
  name: TagKeys
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-remove-tags-request-schema.json
slug: openapi-remove-tags-request
source_filename: openapi-remove-tags-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-remove-tags-request-schema.json\",\n  \"title\": \"RemoveTagsRequest\",\n  \"description\": \"Container for the parameters to the <code><a>RemoveTags</a></code> operation. Specify the <code>ARN</code> for the Elasticsearch domain from which you want to remove the specified <code>TagKey</code>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"Specifies the <code>ARN</code> for the Elasticsearch domain from which you want to delete the specified tags.\"\n        }\n      ]\n    },\n    \"TagKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringList\"\n        },\n        {\n          \"description\": \"Specifies\
  \ the <code>TagKey</code> list which you want to remove from the Elasticsearch domain.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ARN\",\n    \"TagKeys\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-remove-tags-request-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: RemoveTagsRequest
---
