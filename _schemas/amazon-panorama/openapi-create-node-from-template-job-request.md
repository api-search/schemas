---
description: CreateNodeFromTemplateJobRequest schema from Amazon Panorama
layout: schema
name: CreateNodeFromTemplateJobRequest
properties_list:
- description: ''
  name: JobTags
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
  name: TemplateParameters
  type: object
- description: ''
  name: TemplateType
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-create-node-from-template-job-request-schema.json
slug: openapi-create-node-from-template-job-request
source_filename: openapi-create-node-from-template-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-create-node-from-template-job-request-schema.json\",\n  \"title\": \"CreateNodeFromTemplateJobRequest\",\n  \"description\": \"CreateNodeFromTemplateJobRequest schema from Amazon Panorama\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobTagsList\"\n        },\n        {\n          \"description\": \"Tags for the job.\"\n        }\n      ]\n    },\n    \"NodeDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A description for the node.\"\n        }\n      ]\n    },\n    \"NodeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeName\"\n        },\n        {\n\
  \          \"description\": \"A name for the node.\"\n        }\n      ]\n    },\n    \"OutputPackageName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackageName\"\n        },\n        {\n          \"description\": \"An output package name for the node.\"\n        }\n      ]\n    },\n    \"OutputPackageVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodePackageVersion\"\n        },\n        {\n          \"description\": \"An output package version for the node.\"\n        }\n      ]\n    },\n    \"TemplateParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateParametersMap\"\n        },\n        {\n          \"description\": \"Template parameters for the node.\"\n        }\n      ]\n    },\n    \"TemplateType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateType\"\n        },\n        {\n          \"description\": \"The type\
  \ of node.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"NodeName\",\n    \"OutputPackageName\",\n    \"OutputPackageVersion\",\n    \"TemplateParameters\",\n    \"TemplateType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-create-node-from-template-job-request-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: CreateNodeFromTemplateJobRequest
---
