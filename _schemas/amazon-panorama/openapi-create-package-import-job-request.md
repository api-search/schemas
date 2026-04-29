---
description: CreatePackageImportJobRequest schema from Amazon Panorama
layout: schema
name: CreatePackageImportJobRequest
properties_list:
- description: ''
  name: ClientToken
  type: object
- description: ''
  name: InputConfig
  type: object
- description: ''
  name: JobTags
  type: object
- description: ''
  name: JobType
  type: object
- description: ''
  name: OutputConfig
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-create-package-import-job-request-schema.json
slug: openapi-create-package-import-job-request
source_filename: openapi-create-package-import-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-create-package-import-job-request-schema.json\",\n  \"title\": \"CreatePackageImportJobRequest\",\n  \"description\": \"CreatePackageImportJobRequest schema from Amazon Panorama\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"A client token for the package import job.\"\n        }\n      ]\n    },\n    \"InputConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageImportJobInputConfig\"\n        },\n        {\n          \"description\": \"An input config for the package import job.\"\n        }\n      ]\n    },\n    \"JobTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobTagsList\"\
  \n        },\n        {\n          \"description\": \"Tags for the package import job.\"\n        }\n      ]\n    },\n    \"JobType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageImportJobType\"\n        },\n        {\n          \"description\": \"A job type for the package import job.\"\n        }\n      ]\n    },\n    \"OutputConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageImportJobOutputConfig\"\n        },\n        {\n          \"description\": \"An output config for the package import job.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ClientToken\",\n    \"InputConfig\",\n    \"JobType\",\n    \"OutputConfig\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-create-package-import-job-request-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: CreatePackageImportJobRequest
---
