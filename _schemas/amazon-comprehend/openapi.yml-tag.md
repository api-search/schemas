---
description: A key-value pair that adds as a metadata to a resource used by Amazon Comprehend. For example, a tag with the key-value pair ‘Department’:’Sales’ might be added to a resource to indicate its use by a particular department.
layout: schema
name: Tag
properties_list:
- description: ''
  name: Key
  type: object
- description: ''
  name: Value
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-tag-schema.json
slug: openapi.yml-tag
source_filename: openapi.yml-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"A key-value pair that adds as a metadata to a resource used by Amazon Comprehend. For example, a tag with the key-value pair \\u2018Department\\u2019:\\u2019Sales\\u2019 might be added to a resource to indicate its use by a particular department. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagKey\"\n        },\n        {\n          \"description\": \"The initial part of a key-value pair that forms a tag associated with a given resource. For instance, if you want to show which resources are used by which departments, you might use \\u201cDepartment\\u201d as the key portion of the pair, with multiple possible values such as \\u201csales,\\\
  u201d \\u201clegal,\\u201d and \\u201cadministration.\\u201d \"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagValue\"\n        },\n        {\n          \"description\": \" The second part of a key-value pair that forms a tag associated with a given resource. For instance, if you want to show which resources are used by which departments, you might use \\u201cDepartment\\u201d as the initial (key) portion of the pair, with a value of \\u201csales\\u201d to indicate the sales department. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Key\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-tag-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: Tag
---
