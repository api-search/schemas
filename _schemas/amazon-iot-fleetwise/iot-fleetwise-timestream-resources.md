---
description: The registered Amazon Timestream resources that Amazon Web Services IoT FleetWise edge agent software can transfer your vehicle data to.
layout: schema
name: TimestreamResources
properties_list:
- description: ''
  name: timestreamDatabaseName
  type: object
- description: ''
  name: timestreamTableName
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-timestream-resources-schema.json
slug: iot-fleetwise-timestream-resources
source_filename: iot-fleetwise-timestream-resources-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-timestream-resources-schema.json\",\n  \"title\": \"TimestreamResources\",\n  \"description\": \"The registered Amazon Timestream resources that Amazon Web Services IoT FleetWise edge agent software can transfer your vehicle data to.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timestreamDatabaseName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestreamDatabaseName\"\n        },\n        {\n          \"description\": \"The name of the registered Amazon Timestream database.\"\n        }\n      ]\n    },\n    \"timestreamTableName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestreamTableName\"\n        },\n        {\n          \"description\": \"The name of the registered Amazon Timestream database table.\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"timestreamDatabaseName\",\n    \"timestreamTableName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-timestream-resources-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: TimestreamResources
---
