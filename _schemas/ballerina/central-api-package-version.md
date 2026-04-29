---
description: PackageVersion schema from Ballerina Central API
layout: schema
name: PackageVersion
properties_list:
- description: ''
  name: organization
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: version
  type: string
- description: ''
  name: platform
  type: string
- description: ''
  name: ballerinaVersion
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: createdDate
  type: string
- description: ''
  name: modules
  type: array
- description: ''
  name: dependencies
  type: array
provider_name: Ballerina
provider_slug: ballerina
schema_file: json-schema/central-api-package-version-schema.json
slug: central-api-package-version
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ballerina/refs/heads/main/json-schema/central-api-package-version-schema.json\",\n  \"title\": \"PackageVersion\",\n  \"description\": \"PackageVersion schema from Ballerina Central API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"organization\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"version\": {\n      \"type\": \"string\"\n    },\n    \"platform\": {\n      \"type\": \"string\"\n    },\n    \"ballerinaVersion\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"modules\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Module\"\n      }\n    },\n    \"dependencies\": {\n      \"type\"\
  : \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"org\": {\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"version\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ballerina/refs/heads/main/json-schema/central-api-package-version-schema.json
tags:
- Integrations
- Orchestrations
- Open Source
- Programming Language
title: PackageVersion
---
