---
description: StartModelPackagingJobResponse schema from Amazon Lookout for Vision API
layout: schema
name: StartModelPackagingJobResponse
properties_list:
- description: ''
  name: JobName
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-start-model-packaging-job-response-schema.json
slug: amazon-lookout-for-vision-start-model-packaging-job-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-start-model-packaging-job-response-schema.json\",\n  \"title\": \"StartModelPackagingJobResponse\",\n  \"description\": \"StartModelPackagingJobResponse schema from Amazon Lookout for Vision API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelPackagingJobName\"\n        },\n        {\n          \"description\": \"The job name for the model packaging job. If you don't supply a job name in the <code>JobName</code> input parameter, the service creates a job name for you. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-start-model-packaging-job-response-schema.json
tags:
- AWS
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: StartModelPackagingJobResponse
---
