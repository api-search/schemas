---
description: DescribeNodeFromTemplateJobResponse schema from Amazon Panorama
layout: schema
name: DescribeNodeFromTemplateJobResponse
properties_list:
- description: ''
  name: CreatedTime
  type: object
- description: ''
  name: JobId
  type: object
- description: ''
  name: JobTags
  type: object
- description: ''
  name: LastUpdatedTime
  type: object
- description: ''
  name: NodeDescription
  type: object
- description: ''
  name: NodeName
  type: object
- description: ''
  name: OutputPackageName
  type: object
- description: ''
  name: OutputPackageVersion
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: StatusMessage
  type: object
- description: ''
  name: TemplateParameters
  type: object
- description: ''
  name: TemplateType
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-describe-node-from-template-job-response-schema.json
slug: openapi-describe-node-from-template-job-response
source_filename: openapi-describe-node-from-template-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-describe-node-from-template-job-response-schema.json\",\n  \"title\": \"DescribeNodeFromTemplateJobResponse\",\n  \"description\": \"DescribeNodeFromTemplateJobResponse schema from Amazon Panorama\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CreatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedTime\"\n        },\n        {\n          \"description\": \"When the job was created.\"\n        }\n      ]\n    },\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The job's ID.\"\n        }\n      ]\n    },\n    \"JobTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobTagsList\"\n        },\n        {\n     \
  \     \"description\": \"The job's tags.\"\n        }\n      ]\n    },\n    \"LastUpdatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastUpdatedTime\"\n        },\n        {\n          \"description\": \"When the job was updated.\"\n        }\n      ]\n    },\n    \"NodeDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The node's description.\"\n        }\n      ]\n    },\n    \"NodeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeName\"\n        },\n        {\n          \"description\": \"The node's name.\"\n        }\n      ]\n    },\n    \"OutputPackageName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackageName\"\n        },\n        {\n          \"description\": \"The job's output package name.\"\n        }\n      ]\n    },\n    \"OutputPackageVersion\":\
  \ {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackageVersion\"\n        },\n        {\n          \"description\": \"The job's output package version.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeFromTemplateJobStatus\"\n        },\n        {\n          \"description\": \"The job's status.\"\n        }\n      ]\n    },\n    \"StatusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeFromTemplateJobStatusMessage\"\n        },\n        {\n          \"description\": \"The job's status message.\"\n        }\n      ]\n    },\n    \"TemplateParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateParametersMap\"\n        },\n        {\n          \"description\": \"The job's template parameters.\"\n        }\n      ]\n    },\n    \"TemplateType\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/TemplateType\"\n        },\n        {\n          \"description\": \"The job's template type.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CreatedTime\",\n    \"JobId\",\n    \"LastUpdatedTime\",\n    \"NodeName\",\n    \"OutputPackageName\",\n    \"OutputPackageVersion\",\n    \"Status\",\n    \"StatusMessage\",\n    \"TemplateParameters\",\n    \"TemplateType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-describe-node-from-template-job-response-schema.json
tags:
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: DescribeNodeFromTemplateJobResponse
---
