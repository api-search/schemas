---
description: StartModelPackagingJobRequest schema from Amazon Lookout for Vision API
layout: schema
name: StartModelPackagingJobRequest
properties_list:
- description: ''
  name: ModelVersion
  type: object
- description: ''
  name: JobName
  type: object
- description: ''
  name: Configuration
  type: object
- description: ''
  name: Description
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-start-model-packaging-job-request-schema.json
slug: amazon-lookout-for-vision-start-model-packaging-job-request
source_filename: amazon-lookout-for-vision-start-model-packaging-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-start-model-packaging-job-request-schema.json\",\n  \"title\": \"StartModelPackagingJobRequest\",\n  \"description\": \"StartModelPackagingJobRequest schema from Amazon Lookout for Vision API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ModelVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelVersion\"\n        },\n        {\n          \"description\": \" The version of the model within the project that you want to package. \"\n        }\n      ]\n    },\n    \"JobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelPackagingJobName\"\n        },\n        {\n          \"description\": \"A name for the model packaging job. If you don't supply a value, the service creates a job name\
  \ for you. \"\n        }\n      ]\n    },\n    \"Configuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelPackagingConfiguration\"\n        },\n        {\n          \"description\": \"The configuration for the model packaging job. \"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelPackagingJobDescription\"\n        },\n        {\n          \"description\": \"A description for the model packaging job. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ModelVersion\",\n    \"Configuration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-start-model-packaging-job-request-schema.json
tags:
- AWS
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: StartModelPackagingJobRequest
---
