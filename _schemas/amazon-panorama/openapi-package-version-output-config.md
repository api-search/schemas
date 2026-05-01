---
description: A package version output configuration.
layout: schema
name: PackageVersionOutputConfig
properties_list:
- description: ''
  name: MarkLatest
  type: object
- description: ''
  name: PackageName
  type: object
- description: ''
  name: PackageVersion
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-package-version-output-config-schema.json
slug: openapi-package-version-output-config
source_filename: openapi-package-version-output-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-package-version-output-config-schema.json\",\n  \"title\": \"PackageVersionOutputConfig\",\n  \"description\": \"A package version output configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MarkLatest\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MarkLatestPatch\"\n        },\n        {\n          \"description\": \"Indicates that the version is recommended for all users.\"\n        }\n      ]\n    },\n    \"PackageName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackageName\"\n        },\n        {\n          \"description\": \"The output's package name.\"\n        }\n      ]\n    },\n    \"PackageVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackageVersion\"\
  \n        },\n        {\n          \"description\": \"The output's package version.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"PackageName\",\n    \"PackageVersion\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-package-version-output-config-schema.json
tags:
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: PackageVersionOutputConfig
---
