---
description: Contains information about criteria to meet before a job increases its rollout rate. Specify either <code>numberOfNotifiedThings</code> or <code>numberOfSucceededThings</code>.
layout: schema
name: IoTJobRateIncreaseCriteria
properties_list:
- description: ''
  name: numberOfNotifiedThings
  type: object
- description: ''
  name: numberOfSucceededThings
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-io-t-job-rate-increase-criteria-schema.json
slug: iot-greengrass-io-t-job-rate-increase-criteria
source_filename: iot-greengrass-io-t-job-rate-increase-criteria-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-io-t-job-rate-increase-criteria-schema.json\",\n  \"title\": \"IoTJobRateIncreaseCriteria\",\n  \"description\": \"Contains information about criteria to meet before a job increases its rollout rate. Specify either <code>numberOfNotifiedThings</code> or <code>numberOfSucceededThings</code>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"numberOfNotifiedThings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IoTJobNumberOfThings\"\n        },\n        {\n          \"description\": \"The number of devices to receive the job notification before the rollout rate increases.\"\n        }\n      ]\n    },\n    \"numberOfSucceededThings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IoTJobNumberOfThings\"\n        },\n\
  \        {\n          \"description\": \"The number of devices to successfully run the configuration job before the rollout rate increases.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-io-t-job-rate-increase-criteria-schema.json
tags:
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: IoTJobRateIncreaseCriteria
---
