---
description: A package object.
layout: schema
name: PackageObject
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: PackageVersion
  type: object
- description: ''
  name: PatchVersion
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-package-object-schema.json
slug: openapi-package-object
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-package-object-schema.json\",\n  \"title\": \"PackageObject\",\n  \"description\": \"A package object.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackageName\"\n        },\n        {\n          \"description\": \"The object's name.\"\n        }\n      ]\n    },\n    \"PackageVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackageVersion\"\n        },\n        {\n          \"description\": \"The object's package version.\"\n        }\n      ]\n    },\n    \"PatchVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackagePatchVersion\"\n        },\n        {\n          \"description\": \"The object's patch version.\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"PackageVersion\",\n    \"PatchVersion\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-package-object-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: PackageObject
---
