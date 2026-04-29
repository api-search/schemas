---
description: DescribePackageImportJobResponse schema from Amazon Panorama
layout: schema
name: DescribePackageImportJobResponse
properties_list:
- description: ''
  name: ClientToken
  type: object
- description: ''
  name: CreatedTime
  type: object
- description: ''
  name: InputConfig
  type: object
- description: ''
  name: JobId
  type: object
- description: ''
  name: JobTags
  type: object
- description: ''
  name: JobType
  type: object
- description: ''
  name: LastUpdatedTime
  type: object
- description: ''
  name: Output
  type: object
- description: ''
  name: OutputConfig
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: StatusMessage
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-describe-package-import-job-response-schema.json
slug: openapi-describe-package-import-job-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-describe-package-import-job-response-schema.json\",\n  \"title\": \"DescribePackageImportJobResponse\",\n  \"description\": \"DescribePackageImportJobResponse schema from Amazon Panorama\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"The job's client token.\"\n        }\n      ]\n    },\n    \"CreatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedTime\"\n        },\n        {\n          \"description\": \"When the job was created.\"\n        }\n      ]\n    },\n    \"InputConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageImportJobInputConfig\"\
  \n        },\n        {\n          \"description\": \"The job's input config.\"\n        }\n      ]\n    },\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The job's ID.\"\n        }\n      ]\n    },\n    \"JobTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobTagsList\"\n        },\n        {\n          \"description\": \"The job's tags.\"\n        }\n      ]\n    },\n    \"JobType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageImportJobType\"\n        },\n        {\n          \"description\": \"The job's type.\"\n        }\n      ]\n    },\n    \"LastUpdatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastUpdatedTime\"\n        },\n        {\n          \"description\": \"When the job was updated.\"\n        }\n      ]\n    },\n    \"Output\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/PackageImportJobOutput\"\n        },\n        {\n          \"description\": \"The job's output.\"\n        }\n      ]\n    },\n    \"OutputConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageImportJobOutputConfig\"\n        },\n        {\n          \"description\": \"The job's output config.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageImportJobStatus\"\n        },\n        {\n          \"description\": \"The job's status.\"\n        }\n      ]\n    },\n    \"StatusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageImportJobStatusMessage\"\n        },\n        {\n          \"description\": \"The job's status message.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CreatedTime\",\n    \"InputConfig\",\n    \"JobId\",\n    \"JobType\",\n    \"LastUpdatedTime\"\
  ,\n    \"Output\",\n    \"OutputConfig\",\n    \"Status\",\n    \"StatusMessage\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-describe-package-import-job-response-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: DescribePackageImportJobResponse
---
