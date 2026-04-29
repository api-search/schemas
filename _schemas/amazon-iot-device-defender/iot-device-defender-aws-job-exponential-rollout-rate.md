---
description: The rate of increase for a job rollout. This parameter allows you to define an exponential rate increase for a job rollout.
layout: schema
name: AwsJobExponentialRolloutRate
properties_list:
- description: ''
  name: baseRatePerMinute
  type: object
- description: ''
  name: incrementFactor
  type: object
- description: ''
  name: rateIncreaseCriteria
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-aws-job-exponential-rollout-rate-schema.json
slug: iot-device-defender-aws-job-exponential-rollout-rate
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-aws-job-exponential-rollout-rate-schema.json\",\n  \"title\": \"AwsJobExponentialRolloutRate\",\n  \"description\": \"The rate of increase for a job rollout. This parameter allows you to define an exponential rate increase for a job rollout.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"baseRatePerMinute\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsJobRolloutRatePerMinute\"\n        },\n        {\n          \"description\": \"The minimum number of things that will be notified of a pending job, per minute, at the start of the job rollout. This is the initial rate of the rollout.\"\n        }\n      ]\n    },\n    \"incrementFactor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsJobRolloutIncrementFactor\"\
  \n        },\n        {\n          \"description\": \"The rate of increase for a job rollout. The number of things notified is multiplied by this factor.\"\n        }\n      ]\n    },\n    \"rateIncreaseCriteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsJobRateIncreaseCriteria\"\n        },\n        {\n          \"description\": \"<p>The criteria to initiate the increase in rate of rollout for a job.</p> <p>Amazon Web Services IoT Core supports up to one digit after the decimal (for example, 1.5, but not 1.55).</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"baseRatePerMinute\",\n    \"incrementFactor\",\n    \"rateIncreaseCriteria\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-aws-job-exponential-rollout-rate-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: AwsJobExponentialRolloutRate
---
