---
description: ListModelPackagingJobsResponse schema from Amazon Lookout for Vision API
layout: schema
name: ListModelPackagingJobsResponse
properties_list:
- description: ''
  name: ModelPackagingJobs
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-list-model-packaging-jobs-response-schema.json
slug: amazon-lookout-for-vision-list-model-packaging-jobs-response
source_filename: amazon-lookout-for-vision-list-model-packaging-jobs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-list-model-packaging-jobs-response-schema.json\",\n  \"title\": \"ListModelPackagingJobsResponse\",\n  \"description\": \"ListModelPackagingJobsResponse schema from Amazon Lookout for Vision API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ModelPackagingJobs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelPackagingJobsList\"\n        },\n        {\n          \"description\": \" A list of the model packaging jobs created for the specified Amazon Lookout for Vision project. \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"If the previous response was incomplete (because there\
  \ is more results to retrieve), Amazon Lookout for Vision returns a pagination token in the response. You can use this pagination token to retrieve the next set of results. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-list-model-packaging-jobs-response-schema.json
tags:
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: ListModelPackagingJobsResponse
---
