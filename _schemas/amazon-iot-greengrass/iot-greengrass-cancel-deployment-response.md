---
description: CancelDeploymentResponse schema
layout: schema
name: CancelDeploymentResponse
properties_list:
- description: ''
  name: message
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-cancel-deployment-response-schema.json
slug: iot-greengrass-cancel-deployment-response
source_filename: iot-greengrass-cancel-deployment-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-cancel-deployment-response-schema.json\",\n  \"title\": \"CancelDeploymentResponse\",\n  \"description\": \"CancelDeploymentResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"A message that communicates if the cancel was successful.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-cancel-deployment-response-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: CancelDeploymentResponse
---
