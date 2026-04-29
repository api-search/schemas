---
description: Information about the output from a model packaging job.
layout: schema
name: ModelPackagingOutputDetails
properties_list:
- description: ''
  name: Greengrass
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-model-packaging-output-details-schema.json
slug: amazon-lookout-for-vision-model-packaging-output-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-model-packaging-output-details-schema.json\",\n  \"title\": \"ModelPackagingOutputDetails\",\n  \"description\": \" Information about the output from a model packaging job. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Greengrass\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GreengrassOutputDetails\"\n        },\n        {\n          \"description\": \" Information about the AWS IoT Greengrass component in a model packaging job. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-model-packaging-output-details-schema.json
tags:
- AWS
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: ModelPackagingOutputDetails
---
