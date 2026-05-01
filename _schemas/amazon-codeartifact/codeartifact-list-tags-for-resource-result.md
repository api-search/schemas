---
description: ListTagsForResourceResult schema from Amazon CodeArtifact API
layout: schema
name: ListTagsForResourceResult
properties_list:
- description: ''
  name: tags
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-list-tags-for-resource-result-schema.json
slug: codeartifact-list-tags-for-resource-result
source_filename: codeartifact-list-tags-for-resource-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-list-tags-for-resource-result-schema.json\",\n  \"title\": \"ListTagsForResourceResult\",\n  \"description\": \"ListTagsForResourceResult schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"A list of tag key and value pairs associated with the specified resource.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-list-tags-for-resource-result-schema.json
tags:
- Amazon
- Artifact Repository
- Package Management
- DevOps
- Software Supply Chain
- npm
- Maven
- PyPI
- NuGet
title: ListTagsForResourceResult
---
