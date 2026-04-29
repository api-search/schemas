---
description: Container for the parameters to the <code><a>AddTags</a></code> operation. Specify the tags that you want to attach to the Elasticsearch domain.
layout: schema
name: AddTagsRequest
properties_list:
- description: ''
  name: ARN
  type: object
- description: ''
  name: TagList
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-add-tags-request-schema.json
slug: openapi-add-tags-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-add-tags-request-schema.json\",\n  \"title\": \"AddTagsRequest\",\n  \"description\": \"Container for the parameters to the <code><a>AddTags</a></code> operation. Specify the tags that you want to attach to the Elasticsearch domain.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \" Specify the <code>ARN</code> for which you want to add the tags.\"\n        }\n      ]\n    },\n    \"TagList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \" List of <code>Tag</code> that need to be added for the Elasticsearch domain. \"\n        }\n      ]\n    }\n  },\n \
  \ \"required\": [\n    \"ARN\",\n    \"TagList\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-add-tags-request-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: AddTagsRequest
---
