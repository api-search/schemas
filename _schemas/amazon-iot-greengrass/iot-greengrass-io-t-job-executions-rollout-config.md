---
description: Contains information about the rollout configuration for a job. This configuration defines the rate at which the job deploys a configuration to a fleet of target devices.
layout: schema
name: IoTJobExecutionsRolloutConfig
properties_list:
- description: ''
  name: exponentialRate
  type: object
- description: ''
  name: maximumPerMinute
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-io-t-job-executions-rollout-config-schema.json
slug: iot-greengrass-io-t-job-executions-rollout-config
source_filename: iot-greengrass-io-t-job-executions-rollout-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-io-t-job-executions-rollout-config-schema.json\",\n  \"title\": \"IoTJobExecutionsRolloutConfig\",\n  \"description\": \"Contains information about the rollout configuration for a job. This configuration defines the rate at which the job deploys a configuration to a fleet of target devices.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"exponentialRate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IoTJobExponentialRolloutRate\"\n        },\n        {\n          \"description\": \"The exponential rate to increase the job rollout rate.\"\n        }\n      ]\n    },\n    \"maximumPerMinute\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IoTJobMaxExecutionsPerMin\"\n        },\n        {\n          \"description\"\
  : \"The maximum number of devices that receive a pending job notification, per minute.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-io-t-job-executions-rollout-config-schema.json
tags:
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: IoTJobExecutionsRolloutConfig
---
