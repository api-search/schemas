---
description: An output configuration for a package import job.
layout: schema
name: PackageImportJobOutputConfig
properties_list:
- description: ''
  name: PackageVersionOutputConfig
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-package-import-job-output-config-schema.json
slug: openapi-package-import-job-output-config
source_filename: openapi-package-import-job-output-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-package-import-job-output-config-schema.json\",\n  \"title\": \"PackageImportJobOutputConfig\",\n  \"description\": \"An output configuration for a package import job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PackageVersionOutputConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionOutputConfig\"\n        },\n        {\n          \"description\": \"The package version's output configuration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-package-import-job-output-config-schema.json
tags:
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: PackageImportJobOutputConfig
---
