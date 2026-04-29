---
description: A package version input configuration.
layout: schema
name: PackageVersionInputConfig
properties_list:
- description: ''
  name: S3Location
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-package-version-input-config-schema.json
slug: openapi-package-version-input-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-package-version-input-config-schema.json\",\n  \"title\": \"PackageVersionInputConfig\",\n  \"description\": \"A package version input configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3Location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Location\"\n        },\n        {\n          \"description\": \"A location in Amazon S3.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"S3Location\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-package-version-input-config-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: PackageVersionInputConfig
---
