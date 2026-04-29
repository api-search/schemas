---
description: <p>Contains all error-related information for the deployment record. The status details will be null if the deployment is in a success state.</p> <note> <p>Greengrass nucleus v2.8.0 or later is required to get an accurate <code>errorStack</code> and <code>errorTypes</code> response. This field will not be returned for earlier Greengrass nucleus versions.</p> </note>
layout: schema
name: EffectiveDeploymentStatusDetails
properties_list:
- description: ''
  name: errorStack
  type: object
- description: ''
  name: errorTypes
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-effective-deployment-status-details-schema.json
slug: iot-greengrass-effective-deployment-status-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-effective-deployment-status-details-schema.json\",\n  \"title\": \"EffectiveDeploymentStatusDetails\",\n  \"description\": \"<p>Contains all error-related information for the deployment record. The status details will be null if the deployment is in a success state.</p> <note> <p>Greengrass nucleus v2.8.0 or later is required to get an accurate <code>errorStack</code> and <code>errorTypes</code> response. This field will not be returned for earlier Greengrass nucleus versions.</p> </note>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorStack\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EffectiveDeploymentErrorStack\"\n        },\n        {\n          \"description\": \"Contains an ordered list of short error codes that range from the\
  \ most generic error to the most specific one. The error codes describe the reason for failure whenever the <code>coreDeviceExecutionStatus</code> is in a failed state. The response will be an empty list if there is no error.\"\n        }\n      ]\n    },\n    \"errorTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EffectiveDeploymentErrorTypeList\"\n        },\n        {\n          \"description\": \"Contains tags which describe the error. You can use the error types to classify errors to assist with remediating the failure. The response will be an empty list if there is no error.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-effective-deployment-status-details-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: EffectiveDeploymentStatusDetails
---
