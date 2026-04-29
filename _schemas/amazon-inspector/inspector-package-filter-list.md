---
description: PackageFilterList schema
layout: schema
name: PackageFilterList
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-package-filter-list-schema.json
slug: inspector-package-filter-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-package-filter-list-schema.json\",\n  \"title\": \"PackageFilterList\",\n  \"description\": \"PackageFilterList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"architecture\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/StringFilter\"\n          },\n          {\n            \"description\": \"An object that contains details on the package architecture type to filter on.\"\n          }\n        ]\n      },\n      \"epoch\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/NumberFilter\"\n          },\n          {\n            \"description\": \"An object that contains details on the package epoch to filter on.\"\n          }\n        ]\n      },\n      \"name\"\
  : {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/StringFilter\"\n          },\n          {\n            \"description\": \"An object that contains details on the name of the package to filter on.\"\n          }\n        ]\n      },\n      \"release\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/StringFilter\"\n          },\n          {\n            \"description\": \"An object that contains details on the package release to filter on.\"\n          }\n        ]\n      },\n      \"sourceLambdaLayerArn\": {\n        \"$ref\": \"#/components/schemas/StringFilter\"\n      },\n      \"sourceLayerHash\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/StringFilter\"\n          },\n          {\n            \"description\": \"An object that contains details on the source layer hash to filter on.\"\n          }\n        ]\n      },\n      \"version\": {\n        \"allOf\": [\n          {\n\
  \            \"$ref\": \"#/components/schemas/StringFilter\"\n          },\n          {\n            \"description\": \"The package version to filter on.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains information on the details of a package filter.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-package-filter-list-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: PackageFilterList
---
