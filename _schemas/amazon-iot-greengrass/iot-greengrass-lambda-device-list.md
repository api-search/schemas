---
description: LambdaDeviceList schema
layout: schema
name: LambdaDeviceList
properties_list: []
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-lambda-device-list-schema.json
slug: iot-greengrass-lambda-device-list
source_filename: iot-greengrass-lambda-device-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-lambda-device-list-schema.json\",\n  \"title\": \"LambdaDeviceList\",\n  \"description\": \"LambdaDeviceList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"path\"\n    ],\n    \"properties\": {\n      \"path\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/FileSystemPath\"\n          },\n          {\n            \"description\": \"The mount path for the device in the file system.\"\n          }\n        ]\n      },\n      \"permission\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/LambdaFilesystemPermission\"\n          },\n          {\n            \"description\": \"<p>The permission to access the device: read/only (<code>ro</code>) or read/write\
  \ (<code>rw</code>).</p> <p>Default: <code>ro</code> </p>\"\n          }\n        ]\n      },\n      \"addGroupOwner\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/OptionalBoolean\"\n          },\n          {\n            \"description\": \"<p>Whether or not to add the component's system user as an owner of the device.</p> <p>Default: <code>false</code> </p>\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains information about a device that Linux processes in a container can access.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-lambda-device-list-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: LambdaDeviceList
---
