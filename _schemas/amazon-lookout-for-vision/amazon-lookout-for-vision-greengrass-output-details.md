---
description: Information about the AWS IoT Greengrass component created by a model packaging job.
layout: schema
name: GreengrassOutputDetails
properties_list:
- description: ''
  name: ComponentVersionArn
  type: object
- description: ''
  name: ComponentName
  type: object
- description: ''
  name: ComponentVersion
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-greengrass-output-details-schema.json
slug: amazon-lookout-for-vision-greengrass-output-details
source_filename: amazon-lookout-for-vision-greengrass-output-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-greengrass-output-details-schema.json\",\n  \"title\": \"GreengrassOutputDetails\",\n  \"description\": \"Information about the AWS IoT Greengrass component created by a model packaging job. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ComponentVersionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentVersionArn\"\n        },\n        {\n          \"description\": \" The Amazon Resource Name (ARN) of the component. \"\n        }\n      ]\n    },\n    \"ComponentName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentName\"\n        },\n        {\n          \"description\": \" The name of the component. \"\n        }\n      ]\n    },\n    \"ComponentVersion\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/ComponentVersion\"\n        },\n        {\n          \"description\": \" The version of the component. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-greengrass-output-details-schema.json
tags:
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: GreengrassOutputDetails
---
