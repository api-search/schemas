---
description: BatchAssociateClientDeviceWithCoreDeviceRequest schema
layout: schema
name: BatchAssociateClientDeviceWithCoreDeviceRequest
properties_list:
- description: ''
  name: entries
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-batch-associate-client-device-with-core-device-request-schema.json
slug: iot-greengrass-batch-associate-client-device-with-core-device-request
source_filename: iot-greengrass-batch-associate-client-device-with-core-device-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-batch-associate-client-device-with-core-device-request-schema.json\",\n  \"title\": \"BatchAssociateClientDeviceWithCoreDeviceRequest\",\n  \"description\": \"BatchAssociateClientDeviceWithCoreDeviceRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssociateClientDeviceWithCoreDeviceEntryList\"\n        },\n        {\n          \"description\": \"The list of client devices to associate.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-batch-associate-client-device-with-core-device-request-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: BatchAssociateClientDeviceWithCoreDeviceRequest
---
