---
description: <p>Contains criteria that define when and how to cancel a job.</p> <p>The deployment stops if the following conditions are true:</p> <ol> <li> <p>The number of things that receive the deployment exceeds the <code>minNumberOfExecutedThings</code>.</p> </li> <li> <p>The percentage of failures with type <code>failureType</code> exceeds the <code>thresholdPercentage</code>.</p> </li> </ol>
layout: schema
name: IoTJobAbortCriteria
properties_list:
- description: ''
  name: failureType
  type: object
- description: ''
  name: action
  type: object
- description: ''
  name: thresholdPercentage
  type: object
- description: ''
  name: minNumberOfExecutedThings
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-io-t-job-abort-criteria-schema.json
slug: iot-greengrass-io-t-job-abort-criteria
source_filename: iot-greengrass-io-t-job-abort-criteria-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-io-t-job-abort-criteria-schema.json\",\n  \"title\": \"IoTJobAbortCriteria\",\n  \"description\": \"<p>Contains criteria that define when and how to cancel a job.</p> <p>The deployment stops if the following conditions are true:</p> <ol> <li> <p>The number of things that receive the deployment exceeds the <code>minNumberOfExecutedThings</code>.</p> </li> <li> <p>The percentage of failures with type <code>failureType</code> exceeds the <code>thresholdPercentage</code>.</p> </li> </ol>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"failureType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IoTJobExecutionFailureType\"\n        },\n        {\n          \"description\": \"The type of job deployment failure that can cancel a job.\"\n        }\n\
  \      ]\n    },\n    \"action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IoTJobAbortAction\"\n        },\n        {\n          \"description\": \"The action to perform when the criteria are met.\"\n        }\n      ]\n    },\n    \"thresholdPercentage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IoTJobAbortThresholdPercentage\"\n        },\n        {\n          \"description\": \"<p>The minimum percentage of <code>failureType</code> failures that occur before the job can cancel.</p> <p>This parameter supports up to two digits after the decimal (for example, you can specify <code>10.9</code> or <code>10.99</code>, but not <code>10.999</code>).</p>\"\n        }\n      ]\n    },\n    \"minNumberOfExecutedThings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IoTJobMinimumNumberOfExecutedThings\"\n        },\n        {\n          \"description\": \"The minimum number of things that receive\
  \ the configuration before the job can cancel.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"failureType\",\n    \"action\",\n    \"thresholdPercentage\",\n    \"minNumberOfExecutedThings\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-io-t-job-abort-criteria-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: IoTJobAbortCriteria
---
