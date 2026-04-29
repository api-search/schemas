---
description: The destination where the Amazon Web Services IoT FleetWise campaign sends data. You can send data to be stored in Amazon S3 or Amazon Timestream.
layout: schema
name: DataDestinationConfig
properties_list:
- description: ''
  name: s3Config
  type: object
- description: ''
  name: timestreamConfig
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-data-destination-config-schema.json
slug: iot-fleetwise-data-destination-config
source_filename: iot-fleetwise-data-destination-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-data-destination-config-schema.json\",\n  \"title\": \"DataDestinationConfig\",\n  \"description\": \"The destination where the Amazon Web Services IoT FleetWise campaign sends data. You can send data to be stored in Amazon S3 or Amazon Timestream.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"s3Config\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Config\"\n        },\n        {\n          \"description\": \"The Amazon S3 bucket where the Amazon Web Services IoT FleetWise campaign sends data.\"\n        }\n      ]\n    },\n    \"timestreamConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestreamConfig\"\n        },\n        {\n          \"description\": \"The Amazon Timestream table where the campaign\
  \ sends data.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-data-destination-config-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: DataDestinationConfig
---
