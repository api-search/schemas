---
description: A job to import a package version.
layout: schema
name: PackageImportJob
properties_list:
- description: ''
  name: CreatedTime
  type: object
- description: ''
  name: JobId
  type: object
- description: ''
  name: JobType
  type: object
- description: ''
  name: LastUpdatedTime
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: StatusMessage
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-package-import-job-schema.json
slug: openapi-package-import-job
source_filename: openapi-package-import-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-package-import-job-schema.json\",\n  \"title\": \"PackageImportJob\",\n  \"description\": \"A job to import a package version.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CreatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedTime\"\n        },\n        {\n          \"description\": \"When the job was created.\"\n        }\n      ]\n    },\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The job's ID.\"\n        }\n      ]\n    },\n    \"JobType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageImportJobType\"\n        },\n        {\n          \"description\": \"The job's type.\"\n        }\n      ]\n\
  \    },\n    \"LastUpdatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastUpdatedTime\"\n        },\n        {\n          \"description\": \"When the job was updated.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageImportJobStatus\"\n        },\n        {\n          \"description\": \"The job's status.\"\n        }\n      ]\n    },\n    \"StatusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageImportJobStatusMessage\"\n        },\n        {\n          \"description\": \"The job's status message.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-package-import-job-schema.json
tags:
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: PackageImportJob
---
