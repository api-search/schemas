---
description: The log delivery option to send data to Amazon CloudWatch Logs.
layout: schema
name: CloudWatchLogDeliveryOptions
properties_list:
- description: ''
  name: logType
  type: object
- description: ''
  name: logGroupName
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-cloud-watch-log-delivery-options-schema.json
slug: iot-fleetwise-cloud-watch-log-delivery-options
source_filename: iot-fleetwise-cloud-watch-log-delivery-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-cloud-watch-log-delivery-options-schema.json\",\n  \"title\": \"CloudWatchLogDeliveryOptions\",\n  \"description\": \"The log delivery option to send data to Amazon CloudWatch Logs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"logType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogType\"\n        },\n        {\n          \"description\": \"The type of log to send data to Amazon CloudWatch Logs.\"\n        }\n      ]\n    },\n    \"logGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CloudWatchLogGroupName\"\n        },\n        {\n          \"description\": \"The Amazon CloudWatch Logs group the operation sends data to.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"logType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-cloud-watch-log-delivery-options-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: CloudWatchLogDeliveryOptions
---
