---
description: The Lambda function.
layout: schema
name: LambdaFunction
properties_list:
- description: ''
  name: arn
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-lambda-function-schema.json
slug: iot-twinmaker-lambda-function
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-lambda-function-schema.json\",\n  \"title\": \"LambdaFunction\",\n  \"description\": \"The Lambda function.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaArn\"\n        },\n        {\n          \"description\": \"The ARN of the Lambda function.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-lambda-function-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: LambdaFunction
---
