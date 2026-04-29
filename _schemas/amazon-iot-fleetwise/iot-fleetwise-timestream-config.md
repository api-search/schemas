---
description: The Amazon Timestream table where the Amazon Web Services IoT FleetWise campaign sends data. Timestream stores and organizes data to optimize query processing time and to reduce storage costs. For more information, see <a href="https://docs.aws.amazon.com/timestream/latest/developerguide/data-modeling.html">Data modeling</a> in the <i>Amazon Timestream Developer Guide</i>.
layout: schema
name: TimestreamConfig
properties_list:
- description: ''
  name: timestreamTableArn
  type: object
- description: ''
  name: executionRoleArn
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-timestream-config-schema.json
slug: iot-fleetwise-timestream-config
source_filename: iot-fleetwise-timestream-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-timestream-config-schema.json\",\n  \"title\": \"TimestreamConfig\",\n  \"description\": \"The Amazon Timestream table where the Amazon Web Services IoT FleetWise campaign sends data. Timestream stores and organizes data to optimize query processing time and to reduce storage costs. For more information, see <a href=\\\"https://docs.aws.amazon.com/timestream/latest/developerguide/data-modeling.html\\\">Data modeling</a> in the <i>Amazon Timestream Developer Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timestreamTableArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestreamTableArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Amazon Timestream table.\"\n        }\n      ]\n    },\n\
  \    \"executionRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IAMRoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the task execution role that grants Amazon Web Services IoT FleetWise permission to deliver data to the Amazon Timestream table.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"timestreamTableArn\",\n    \"executionRoleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-timestream-config-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: TimestreamConfig
---
