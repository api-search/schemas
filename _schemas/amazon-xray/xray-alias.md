---
description: An alias for an edge.
layout: schema
name: Alias
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Names
  type: object
- description: ''
  name: Type
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-alias-schema.json
slug: xray-alias
source_filename: xray-alias-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The canonical name of the alias.\"\n        }\n      ]\n    },\n    \"Names\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AliasNames\"\n        },\n        {\n          \"description\": \"A list of names for the alias, including the canonical name.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The type of the alias.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An alias for an edge.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Alias\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-alias-schema.json\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-alias-schema.json
tags:
- Application Performance
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: Alias
---
