---
description: Results of a package import job.
layout: schema
name: PackageImportJobOutput
properties_list:
- description: ''
  name: OutputS3Location
  type: object
- description: ''
  name: PackageId
  type: object
- description: ''
  name: PackageVersion
  type: object
- description: ''
  name: PatchVersion
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-package-import-job-output-schema.json
slug: openapi-package-import-job-output
source_filename: openapi-package-import-job-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-package-import-job-output-schema.json\",\n  \"title\": \"PackageImportJobOutput\",\n  \"description\": \"Results of a package import job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OutputS3Location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutPutS3Location\"\n        },\n        {\n          \"description\": \"The package's output location.\"\n        }\n      ]\n    },\n    \"PackageId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackageId\"\n        },\n        {\n          \"description\": \"The package's ID.\"\n        }\n      ]\n    },\n    \"PackageVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackageVersion\"\n        },\n        {\n          \"description\"\
  : \"The package's version.\"\n        }\n      ]\n    },\n    \"PatchVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackagePatchVersion\"\n        },\n        {\n          \"description\": \"The package's patch version.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"OutputS3Location\",\n    \"PackageId\",\n    \"PackageVersion\",\n    \"PatchVersion\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-package-import-job-output-schema.json
tags:
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: PackageImportJobOutput
---
