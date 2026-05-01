---
description: UntagResourceRequest schema
layout: schema
name: UntagResourceRequest
properties_list:
- description: ''
  name: ResourceArn
  type: object
- description: ''
  name: TagKeys
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-untag-resource-request-schema.json
slug: openapi.yml-untag-resource-request
source_filename: openapi.yml-untag-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-untag-resource-request-schema.json\",\n  \"title\": \"UntagResourceRequest\",\n  \"description\": \"UntagResourceRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendArn\"\n        },\n        {\n          \"description\": \" The Amazon Resource Name (ARN) of the given Amazon Comprehend resource from which you want to remove the tags. \"\n        }\n      ]\n    },\n    \"TagKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagKeyList\"\n        },\n        {\n          \"description\": \"The initial part of a key-value pair that forms a tag being removed from a given resource. For example, a tag with \\\"Sales\\\" as the key might be added\
  \ to a resource to indicate its use by the sales department. Keys must be unique and cannot be duplicated for a particular resource. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceArn\",\n    \"TagKeys\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-untag-resource-request-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: UntagResourceRequest
---
