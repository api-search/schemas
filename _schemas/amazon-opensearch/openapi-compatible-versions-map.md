---
description: A map from an <code> <a>ElasticsearchVersion</a> </code> to a list of compatible <code> <a>ElasticsearchVersion</a> </code> s to which the domain can be upgraded.
layout: schema
name: CompatibleVersionsMap
properties_list:
- description: ''
  name: SourceVersion
  type: object
- description: ''
  name: TargetVersions
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-compatible-versions-map-schema.json
slug: openapi-compatible-versions-map
source_filename: openapi-compatible-versions-map-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-compatible-versions-map-schema.json\",\n  \"title\": \"CompatibleVersionsMap\",\n  \"description\": \" A map from an <code> <a>ElasticsearchVersion</a> </code> to a list of compatible <code> <a>ElasticsearchVersion</a> </code> s to which the domain can be upgraded. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SourceVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ElasticsearchVersionString\"\n        },\n        {\n          \"description\": \"The current version of Elasticsearch on which a domain is.\"\n        }\n      ]\n    },\n    \"TargetVersions\": {\n      \"$ref\": \"#/components/schemas/ElasticsearchVersionList\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-compatible-versions-map-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: CompatibleVersionsMap
---
