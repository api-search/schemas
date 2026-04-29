---
description: PackageDocs schema from Ballerina Central API
layout: schema
name: PackageDocs
properties_list:
- description: ''
  name: modules
  type: array
provider_name: Ballerina
provider_slug: ballerina
schema_file: json-schema/central-api-package-docs-schema.json
slug: central-api-package-docs
source_filename: central-api-package-docs-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ballerina/refs/heads/main/json-schema/central-api-package-docs-schema.json\",\n  \"title\": \"PackageDocs\",\n  \"description\": \"PackageDocs schema from Ballerina Central API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"modules\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"description\": {\n            \"type\": \"string\"\n          },\n          \"functions\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"name\": {\n                  \"type\": \"string\"\n                },\n                \"description\": {\n                  \"type\": \"string\"\n                },\n           \
  \     \"isIsolated\": {\n                  \"type\": \"boolean\"\n                }\n              }\n            }\n          },\n          \"classes\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"name\": {\n                  \"type\": \"string\"\n                },\n                \"description\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          },\n          \"records\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"name\": {\n                  \"type\": \"string\"\n                },\n                \"description\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          },\n          \"types\": {\n            \"type\": \"array\",\n            \"items\": {\n            \
  \  \"type\": \"object\",\n              \"properties\": {\n                \"name\": {\n                  \"type\": \"string\"\n                },\n                \"description\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          },\n          \"errors\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"name\": {\n                  \"type\": \"string\"\n                },\n                \"description\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ballerina/refs/heads/main/json-schema/central-api-package-docs-schema.json
tags:
- Integrations
- Orchestrations
- Open Source
- Programming Language
title: PackageDocs
---
