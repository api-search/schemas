---
description: Allows you to create an exponential rate of rollout for a job.
layout: schema
name: ExponentialRolloutRate
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
schema_file: json-schema/iot-device-defender-exponential-rollout-rate-schema.json
slug: iot-device-defender-exponential-rollout-rate
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-exponential-rollout-rate-schema.json\",\n  \"title\": \"ExponentialRolloutRate\",\n  \"description\": \"Allows you to create an exponential rate of rollout for a job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"baseRatePerMinute\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RolloutRatePerMinute\"\n        },\n        {\n          \"description\": \"The minimum number of things that will be notified of a pending job, per minute at the start of job rollout. This parameter allows you to define the initial rate of rollout.\"\n        }\n      ]\n    },\n    \"incrementFactor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IncrementFactor\"\n        },\n        {\n          \"description\": \"<p>The\
  \ exponential factor to increase the rate of rollout for a job.</p> <p>Amazon Web Services IoT Core supports up to one digit after the decimal (for example, 1.5, but not 1.55).</p>\"\n        }\n      ]\n    },\n    \"rateIncreaseCriteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RateIncreaseCriteria\"\n        },\n        {\n          \"description\": \"The criteria to initiate the increase in rate of rollout for a job.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"baseRatePerMinute\",\n    \"incrementFactor\",\n    \"rateIncreaseCriteria\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-exponential-rollout-rate-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: ExponentialRolloutRate
---
