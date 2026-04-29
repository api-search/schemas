---
description: A filter used to limit results when describing inbound or outbound cross-cluster search connections. Multiple values can be specified per filter. A cross-cluster search connection must match at least one of the specified values for it to be returned from an operation.
layout: schema
name: Filter
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Values
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-filter-schema.json
slug: openapi-filter
source_filename: openapi-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-filter-schema.json\",\n  \"title\": \"Filter\",\n  \"description\": \" A filter used to limit results when describing inbound or outbound cross-cluster search connections. Multiple values can be specified per filter. A cross-cluster search connection must match at least one of the specified values for it to be returned from an operation. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \" Specifies the name of the filter. \"\n        }\n      ]\n    },\n    \"Values\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ValueStringList\"\n        },\n        {\n          \"description\": \" Contains one or more\
  \ values for the filter. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-filter-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: Filter
---
