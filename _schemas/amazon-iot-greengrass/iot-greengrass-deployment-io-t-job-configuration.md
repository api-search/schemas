---
description: Contains information about an IoT job configuration.
layout: schema
name: DeploymentIoTJobConfiguration
properties_list:
- description: ''
  name: jobExecutionsRolloutConfig
  type: object
- description: ''
  name: abortConfig
  type: object
- description: ''
  name: timeoutConfig
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-deployment-io-t-job-configuration-schema.json
slug: iot-greengrass-deployment-io-t-job-configuration
source_filename: iot-greengrass-deployment-io-t-job-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-deployment-io-t-job-configuration-schema.json\",\n  \"title\": \"DeploymentIoTJobConfiguration\",\n  \"description\": \"Contains information about an IoT job configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobExecutionsRolloutConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IoTJobExecutionsRolloutConfig\"\n        },\n        {\n          \"description\": \"The rollout configuration for the job. This configuration defines the rate at which the job rolls out to the fleet of target devices.\"\n        }\n      ]\n    },\n    \"abortConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IoTJobAbortConfig\"\n        },\n        {\n          \"description\": \"The stop configuration for the job.\
  \ This configuration defines when and how to stop a job rollout.\"\n        }\n      ]\n    },\n    \"timeoutConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IoTJobTimeoutConfig\"\n        },\n        {\n          \"description\": \"The timeout configuration for the job. This configuration defines the amount of time each device has to complete the job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-deployment-io-t-job-configuration-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: DeploymentIoTJobConfiguration
---
