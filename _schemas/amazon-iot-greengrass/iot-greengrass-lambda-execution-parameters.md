---
description: Contains parameters for a Lambda function that runs on IoT Greengrass.
layout: schema
name: LambdaExecutionParameters
properties_list:
- description: ''
  name: eventSources
  type: object
- description: ''
  name: maxQueueSize
  type: object
- description: ''
  name: maxInstancesCount
  type: object
- description: ''
  name: maxIdleTimeInSeconds
  type: object
- description: ''
  name: timeoutInSeconds
  type: object
- description: ''
  name: statusTimeoutInSeconds
  type: object
- description: ''
  name: pinned
  type: object
- description: ''
  name: inputPayloadEncodingType
  type: object
- description: ''
  name: execArgs
  type: object
- description: ''
  name: environmentVariables
  type: object
- description: ''
  name: linuxProcessParams
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-lambda-execution-parameters-schema.json
slug: iot-greengrass-lambda-execution-parameters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-lambda-execution-parameters-schema.json\",\n  \"title\": \"LambdaExecutionParameters\",\n  \"description\": \"Contains parameters for a Lambda function that runs on IoT Greengrass.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventSources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaEventSourceList\"\n        },\n        {\n          \"description\": \"The list of event sources to which to subscribe to receive work messages. The Lambda function runs when it receives a message from an event source. You can subscribe this function to local publish/subscribe messages and Amazon Web Services IoT Core MQTT messages.\"\n        }\n      ]\n    },\n    \"maxQueueSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OptionalInteger\"\
  \n        },\n        {\n          \"description\": \"The maximum size of the message queue for the Lambda function component. The IoT Greengrass core stores messages in a FIFO (first-in-first-out) queue until it can run the Lambda function to consume each message.\"\n        }\n      ]\n    },\n    \"maxInstancesCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OptionalInteger\"\n        },\n        {\n          \"description\": \"The maximum number of instances that a non-pinned Lambda function can run at the same time.\"\n        }\n      ]\n    },\n    \"maxIdleTimeInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OptionalInteger\"\n        },\n        {\n          \"description\": \"The maximum amount of time in seconds that a non-pinned Lambda function can idle before the IoT Greengrass Core software stops its process.\"\n        }\n      ]\n    },\n    \"timeoutInSeconds\": {\n      \"allOf\": [\n      \
  \  {\n          \"$ref\": \"#/components/schemas/OptionalInteger\"\n        },\n        {\n          \"description\": \"The maximum amount of time in seconds that the Lambda function can process a work item.\"\n        }\n      ]\n    },\n    \"statusTimeoutInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OptionalInteger\"\n        },\n        {\n          \"description\": \"The interval in seconds at which a pinned (also known as long-lived) Lambda function component sends status updates to the Lambda manager component.\"\n        }\n      ]\n    },\n    \"pinned\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OptionalBoolean\"\n        },\n        {\n          \"description\": \"<p>Whether or not the Lambda function is pinned, or long-lived.</p> <ul> <li> <p>A pinned Lambda function starts when IoT Greengrass starts and keeps running in its own container.</p> </li> <li> <p>A non-pinned Lambda function starts only\
  \ when it receives a work item and exists after it idles for <code>maxIdleTimeInSeconds</code>. If the function has multiple work items, the IoT Greengrass Core software creates multiple instances of the function.</p> </li> </ul> <p>Default: <code>true</code> </p>\"\n        }\n      ]\n    },\n    \"inputPayloadEncodingType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaInputPayloadEncodingType\"\n        },\n        {\n          \"description\": \"<p>The encoding type that the Lambda function supports.</p> <p>Default: <code>json</code> </p>\"\n        }\n      ]\n    },\n    \"execArgs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaExecArgsList\"\n        },\n        {\n          \"description\": \"The list of arguments to pass to the Lambda function when it runs.\"\n        }\n      ]\n    },\n    \"environmentVariables\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaEnvironmentVariables\"\
  \n        },\n        {\n          \"description\": \"The map of environment variables that are available to the Lambda function when it runs.\"\n        }\n      ]\n    },\n    \"linuxProcessParams\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaLinuxProcessParams\"\n        },\n        {\n          \"description\": \"The parameters for the Linux process that contains the Lambda function.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-lambda-execution-parameters-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: LambdaExecutionParameters
---
