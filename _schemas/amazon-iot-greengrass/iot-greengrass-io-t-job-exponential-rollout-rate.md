---
description: Contains information about an exponential rollout rate for a configuration deployment job.
layout: schema
name: IoTJobExponentialRolloutRate
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
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-io-t-job-exponential-rollout-rate-schema.json
slug: iot-greengrass-io-t-job-exponential-rollout-rate
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-io-t-job-exponential-rollout-rate-schema.json\",\n  \"title\": \"IoTJobExponentialRolloutRate\",\n  \"description\": \"Contains information about an exponential rollout rate for a configuration deployment job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"baseRatePerMinute\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IoTJobRolloutBaseRatePerMinute\"\n        },\n        {\n          \"description\": \"The minimum number of devices that receive a pending job notification, per minute, when the job starts. This parameter defines the initial rollout rate of the job.\"\n        }\n      ]\n    },\n    \"incrementFactor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IoTJobRolloutIncrementFactor\"\n        },\n\
  \        {\n          \"description\": \"<p>The exponential factor to increase the rollout rate for the job.</p> <p>This parameter supports up to one digit after the decimal (for example, you can specify <code>1.5</code>, but not <code>1.55</code>).</p>\"\n        }\n      ]\n    },\n    \"rateIncreaseCriteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IoTJobRateIncreaseCriteria\"\n        },\n        {\n          \"description\": \"The criteria to increase the rollout rate for the job.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"baseRatePerMinute\",\n    \"incrementFactor\",\n    \"rateIncreaseCriteria\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-io-t-job-exponential-rollout-rate-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: IoTJobExponentialRolloutRate
---
