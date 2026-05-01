---
description: BatchDisassociateClientDeviceFromCoreDeviceResponse schema
layout: schema
name: BatchDisassociateClientDeviceFromCoreDeviceResponse
properties_list:
- description: ''
  name: errorEntries
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-batch-disassociate-client-device-from-core-device-response-schema.json
slug: iot-greengrass-batch-disassociate-client-device-from-core-device-response
source_filename: iot-greengrass-batch-disassociate-client-device-from-core-device-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-batch-disassociate-client-device-from-core-device-response-schema.json\",\n  \"title\": \"BatchDisassociateClientDeviceFromCoreDeviceResponse\",\n  \"description\": \"BatchDisassociateClientDeviceFromCoreDeviceResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorEntries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DisassociateClientDeviceFromCoreDeviceErrorList\"\n        },\n        {\n          \"description\": \"The list of any errors for the entries in the request. Each error entry contains the name of the IoT thing that failed to disassociate.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-batch-disassociate-client-device-from-core-device-response-schema.json
tags:
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: BatchDisassociateClientDeviceFromCoreDeviceResponse
---
