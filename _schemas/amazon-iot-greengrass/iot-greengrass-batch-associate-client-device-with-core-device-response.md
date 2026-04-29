---
description: BatchAssociateClientDeviceWithCoreDeviceResponse schema
layout: schema
name: BatchAssociateClientDeviceWithCoreDeviceResponse
properties_list:
- description: ''
  name: errorEntries
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-batch-associate-client-device-with-core-device-response-schema.json
slug: iot-greengrass-batch-associate-client-device-with-core-device-response
source_filename: iot-greengrass-batch-associate-client-device-with-core-device-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-batch-associate-client-device-with-core-device-response-schema.json\",\n  \"title\": \"BatchAssociateClientDeviceWithCoreDeviceResponse\",\n  \"description\": \"BatchAssociateClientDeviceWithCoreDeviceResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorEntries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssociateClientDeviceWithCoreDeviceErrorList\"\n        },\n        {\n          \"description\": \"The list of any errors for the entries in the request. Each error entry contains the name of the IoT thing that failed to associate.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-batch-associate-client-device-with-core-device-response-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: BatchAssociateClientDeviceWithCoreDeviceResponse
---
