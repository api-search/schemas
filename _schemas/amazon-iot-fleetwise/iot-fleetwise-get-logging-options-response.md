---
description: GetLoggingOptionsResponse schema
layout: schema
name: GetLoggingOptionsResponse
properties_list:
- description: ''
  name: cloudWatchLogDelivery
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-get-logging-options-response-schema.json
slug: iot-fleetwise-get-logging-options-response
source_filename: iot-fleetwise-get-logging-options-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-get-logging-options-response-schema.json\",\n  \"title\": \"GetLoggingOptionsResponse\",\n  \"description\": \"GetLoggingOptionsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cloudWatchLogDelivery\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CloudWatchLogDeliveryOptions\"\n        },\n        {\n          \"description\": \"Returns information about log delivery to Amazon CloudWatch Logs.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"cloudWatchLogDelivery\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-get-logging-options-response-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: GetLoggingOptionsResponse
---
