---
description: Contains information about a deployment job that IoT Greengrass sends to a Greengrass core device.
layout: schema
name: EffectiveDeployment
properties_list:
- description: ''
  name: deploymentId
  type: object
- description: ''
  name: deploymentName
  type: object
- description: ''
  name: iotJobId
  type: object
- description: ''
  name: iotJobArn
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: targetArn
  type: object
- description: ''
  name: coreDeviceExecutionStatus
  type: object
- description: ''
  name: reason
  type: object
- description: ''
  name: creationTimestamp
  type: object
- description: ''
  name: modifiedTimestamp
  type: object
- description: ''
  name: statusDetails
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-effective-deployment-schema.json
slug: iot-greengrass-effective-deployment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-effective-deployment-schema.json\",\n  \"title\": \"EffectiveDeployment\",\n  \"description\": \"Contains information about a deployment job that IoT Greengrass sends to a Greengrass core device.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentID\"\n        },\n        {\n          \"description\": \"The ID of the deployment.\"\n        }\n      ]\n    },\n    \"deploymentName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentName\"\n        },\n        {\n          \"description\": \"The name of the deployment.\"\n        }\n      ]\n    },\n    \"iotJobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IoTJobId\"\
  \n        },\n        {\n          \"description\": \"The ID of the IoT job that applies the deployment to target devices.\"\n        }\n      ]\n    },\n    \"iotJobArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IoTJobARN\"\n        },\n        {\n          \"description\": \"The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the IoT job that applies the deployment to target devices.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The description of the deployment job.\"\n        }\n      ]\n    },\n    \"targetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetARN\"\n        },\n        {\n          \"description\": \"The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\"\
  >ARN</a> of the target IoT thing or thing group.\"\n        }\n      ]\n    },\n    \"coreDeviceExecutionStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EffectiveDeploymentExecutionStatus\"\n        },\n        {\n          \"description\": \"<p>The status of the deployment job on the Greengrass core device.</p> <ul> <li> <p> <code>IN_PROGRESS</code> \\u2013 The deployment job is running.</p> </li> <li> <p> <code>QUEUED</code> \\u2013 The deployment job is in the job queue and waiting to run.</p> </li> <li> <p> <code>FAILED</code> \\u2013 The deployment failed. For more information, see the <code>statusDetails</code> field.</p> </li> <li> <p> <code>COMPLETED</code> \\u2013 The deployment to an IoT thing was completed successfully.</p> </li> <li> <p> <code>TIMED_OUT</code> \\u2013 The deployment didn't complete in the allotted time. </p> </li> <li> <p> <code>CANCELED</code> \\u2013 The deployment was canceled by the user.</p> </li> <li> <p> <code>REJECTED</code>\
  \ \\u2013 The deployment was rejected. For more information, see the <code>statusDetails</code> field.</p> </li> <li> <p> <code>SUCCEEDED</code> \\u2013 The deployment to an IoT thing group was completed successfully.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"reason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Reason\"\n        },\n        {\n          \"description\": \"The reason code for the update, if the job was updated.\"\n        }\n      ]\n    },\n    \"creationTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at which the deployment was created, expressed in ISO 8601 format.\"\n        }\n      ]\n    },\n    \"modifiedTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at which the deployment job was last modified,\
  \ expressed in ISO 8601 format.\"\n        }\n      ]\n    },\n    \"statusDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EffectiveDeploymentStatusDetails\"\n        },\n        {\n          \"description\": \"The status details that explain why a deployment has an error. This response will be null if the deployment is in a success state.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"deploymentId\",\n    \"deploymentName\",\n    \"targetArn\",\n    \"coreDeviceExecutionStatus\",\n    \"creationTimestamp\",\n    \"modifiedTimestamp\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-effective-deployment-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: EffectiveDeployment
---
