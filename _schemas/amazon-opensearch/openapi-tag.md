---
description: Specifies a key value pair for a resource tag.
layout: schema
name: Tag
properties_list:
- description: ''
  name: Key
  type: object
- description: ''
  name: Value
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-tag-schema.json
slug: openapi-tag
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"Specifies a key value pair for a resource tag.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagKey\"\n        },\n        {\n          \"description\": \"Specifies the <code>TagKey</code>, the name of the tag. Tag keys must be unique for the Elasticsearch domain to which they are attached.\"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagValue\"\n        },\n        {\n          \"description\": \"Specifies the <code>TagValue</code>, the value assigned to the corresponding tag key. Tag values can be null and do not have to be unique in a tag set. For example, you\
  \ can have a key value pair in a tag set of <code>project : Trinity</code> and <code>cost-center : Trinity</code>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Key\",\n    \"Value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-tag-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: Tag
---
