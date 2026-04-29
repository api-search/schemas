---
description: Contains information about the timeout configuration for a job.
layout: schema
name: IoTJobTimeoutConfig
properties_list:
- description: ''
  name: inProgressTimeoutInMinutes
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-io-t-job-timeout-config-schema.json
slug: iot-greengrass-io-t-job-timeout-config
source_filename: iot-greengrass-io-t-job-timeout-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-io-t-job-timeout-config-schema.json\",\n  \"title\": \"IoTJobTimeoutConfig\",\n  \"description\": \"Contains information about the timeout configuration for a job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inProgressTimeoutInMinutes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IoTJobInProgressTimeoutInMinutes\"\n        },\n        {\n          \"description\": \"<p>The amount of time, in minutes, that devices have to complete the job. The timer starts when the job status is set to <code>IN_PROGRESS</code>. If the job status doesn't change to a terminal state before the time expires, then the job status is set to <code>TIMED_OUT</code>.</p> <p>The timeout interval must be between 1 minute and 7 days (10080 minutes).</p>\"\n        }\n\
  \      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-io-t-job-timeout-config-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: IoTJobTimeoutConfig
---
