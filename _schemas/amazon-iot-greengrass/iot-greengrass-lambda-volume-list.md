---
description: LambdaVolumeList schema
layout: schema
name: LambdaVolumeList
properties_list: []
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-lambda-volume-list-schema.json
slug: iot-greengrass-lambda-volume-list
source_filename: iot-greengrass-lambda-volume-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-lambda-volume-list-schema.json\",\n  \"title\": \"LambdaVolumeList\",\n  \"description\": \"LambdaVolumeList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"sourcePath\",\n      \"destinationPath\"\n    ],\n    \"properties\": {\n      \"sourcePath\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/FileSystemPath\"\n          },\n          {\n            \"description\": \"The path to the physical volume in the file system.\"\n          }\n        ]\n      },\n      \"destinationPath\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/FileSystemPath\"\n          },\n          {\n            \"description\": \"The path to the logical volume in the file system.\"\
  \n          }\n        ]\n      },\n      \"permission\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/LambdaFilesystemPermission\"\n          },\n          {\n            \"description\": \"<p>The permission to access the volume: read/only (<code>ro</code>) or read/write (<code>rw</code>).</p> <p>Default: <code>ro</code> </p>\"\n          }\n        ]\n      },\n      \"addGroupOwner\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/OptionalBoolean\"\n          },\n          {\n            \"description\": \"<p>Whether or not to add the IoT Greengrass user group as an owner of the volume.</p> <p>Default: <code>false</code> </p>\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains information about a volume that Linux processes in a container can access. When you define a volume, the IoT Greengrass Core software mounts the source files to the destination inside the container.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-lambda-volume-list-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: LambdaVolumeList
---
