---
description: Schema representing an SDK generation request and result in APIMatic
layout: schema
name: APIMatic SDK Generation
properties_list:
- description: Target SDK platform for code generation
  name: platform
  type: string
- description: URL to download the generated SDK package
  name: downloadUrl
  type: string
- description: Expiration timestamp for the download URL
  name: expiresAt
  type: string
provider_name: APIMatic
provider_slug: apimatic
schema_file: json-schema/apimatic-sdk-generation-schema.json
slug: apimatic-sdk-generation
source_filename: apimatic-sdk-generation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apimatic/main/json-schema/apimatic-sdk-generation-schema.json\",\n  \"title\": \"APIMatic SDK Generation\",\n  \"description\": \"Schema representing an SDK generation request and result in APIMatic\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"platform\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CS_NET_STANDARD_LIB\",\n        \"JAVA_ECLIPSE_JRE_LIB\",\n        \"PHP_GENERIC_LIB\",\n        \"PYTHON_GENERIC_LIB\",\n        \"RUBY_GENERIC_LIB\",\n        \"TYPESCRIPT_GENERIC_LIB\",\n        \"GO_GENERIC_LIB\"\n      ],\n      \"description\": \"Target SDK platform for code generation\"\n    },\n    \"downloadUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to download the generated SDK package\"\n    },\n    \"expiresAt\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"date-time\",\n      \"description\": \"Expiration timestamp for the download URL\"\n    }\n  },\n  \"required\": [\"platform\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/json-schema/apimatic-sdk-generation-schema.json
tags:
- API Transformation
- Code Generation
- Developer Experience
- Documentation
- SDK Generation
title: APIMatic SDK Generation
---
