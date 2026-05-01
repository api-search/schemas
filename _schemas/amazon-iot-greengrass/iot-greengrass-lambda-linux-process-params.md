---
description: Contains parameters for a Linux process that contains an Lambda function.
layout: schema
name: LambdaLinuxProcessParams
properties_list:
- description: ''
  name: isolationMode
  type: object
- description: ''
  name: containerParams
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-lambda-linux-process-params-schema.json
slug: iot-greengrass-lambda-linux-process-params
source_filename: iot-greengrass-lambda-linux-process-params-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-lambda-linux-process-params-schema.json\",\n  \"title\": \"LambdaLinuxProcessParams\",\n  \"description\": \"Contains parameters for a Linux process that contains an Lambda function.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"isolationMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaIsolationMode\"\n        },\n        {\n          \"description\": \"<p>The isolation mode for the process that contains the Lambda function. The process can run in an isolated runtime environment inside the IoT Greengrass container, or as a regular process outside any container.</p> <p>Default: <code>GreengrassContainer</code> </p>\"\n        }\n      ]\n    },\n    \"containerParams\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaContainerParams\"\
  \n        },\n        {\n          \"description\": \"The parameters for the container in which the Lambda function runs.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-lambda-linux-process-params-schema.json
tags:
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: LambdaLinuxProcessParams
---
