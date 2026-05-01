---
description: CreatePackageRequest schema from Amazon Panorama
layout: schema
name: CreatePackageRequest
properties_list:
- description: ''
  name: PackageName
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-create-package-request-schema.json
slug: openapi-create-package-request
source_filename: openapi-create-package-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-create-package-request-schema.json\",\n  \"title\": \"CreatePackageRequest\",\n  \"description\": \"CreatePackageRequest schema from Amazon Panorama\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PackageName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackageName\"\n        },\n        {\n          \"description\": \"A name for the package.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Tags for the package.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"PackageName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-create-package-request-schema.json
tags:
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: CreatePackageRequest
---
