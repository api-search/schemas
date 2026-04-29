---
description: CreateDeploymentResponse schema
layout: schema
name: CreateDeploymentResponse
properties_list:
- description: ''
  name: deploymentId
  type: object
- description: ''
  name: iotJobId
  type: object
- description: ''
  name: iotJobArn
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-create-deployment-response-schema.json
slug: iot-greengrass-create-deployment-response
source_filename: iot-greengrass-create-deployment-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-create-deployment-response-schema.json\",\n  \"title\": \"CreateDeploymentResponse\",\n  \"description\": \"CreateDeploymentResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The ID of the deployment.\"\n        }\n      ]\n    },\n    \"iotJobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The ID of the IoT job that applies the deployment to target devices.\"\n        }\n      ]\n    },\n    \"iotJobArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IoTJobARN\"\n \
  \       },\n        {\n          \"description\": \"The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the IoT job that applies the deployment to target devices.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-create-deployment-response-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: CreateDeploymentResponse
---
