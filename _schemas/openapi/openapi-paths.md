---
description: Holds the relative paths to the individual endpoints and their operations. The path is appended to the URL from the Server Object to construct the full URL.
layout: schema
name: OpenAPI Paths Object
properties_list: []
provider_name: OpenAPI
provider_slug: openapi
schema_file: json-schema/openapi-paths.json
slug: openapi-paths
source_filename: openapi-paths.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"openapi-paths.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OpenAPI Paths Object\",\n  \"description\": \"Holds the relative paths to the individual endpoints and their operations. The path is appended to the URL from the Server Object to construct the full URL.\",\n  \"type\": \"object\",\n  \"patternProperties\": {\n    \"^\\\\/\": {\n      \"$ref\": \"openapi-path-item.json\"\n    },\n    \"^x-\": {}\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openapi/refs/heads/main/json-schema/openapi-paths.json
tags:
- Documentation
- REST
- Specification
title: OpenAPI Paths Object
---
