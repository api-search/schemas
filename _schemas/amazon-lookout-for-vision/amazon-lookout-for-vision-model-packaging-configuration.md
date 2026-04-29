---
description: Configuration information for a Amazon Lookout for Vision model packaging job. For more information, see <a>StartModelPackagingJob</a>.
layout: schema
name: ModelPackagingConfiguration
properties_list:
- description: ''
  name: Greengrass
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-model-packaging-configuration-schema.json
slug: amazon-lookout-for-vision-model-packaging-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-model-packaging-configuration-schema.json\",\n  \"title\": \"ModelPackagingConfiguration\",\n  \"description\": \" Configuration information for a Amazon Lookout for Vision model packaging job. For more information, see <a>StartModelPackagingJob</a>. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Greengrass\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GreengrassConfiguration\"\n        },\n        {\n          \"description\": \" Configuration information for the AWS IoT Greengrass component in a model packaging job. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Greengrass\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-model-packaging-configuration-schema.json
tags:
- AWS
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: ModelPackagingConfiguration
---
