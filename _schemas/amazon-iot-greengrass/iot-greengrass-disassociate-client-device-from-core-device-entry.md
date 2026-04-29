---
description: Contains a request to disassociate a client device from a core device. The <a href="https://docs.aws.amazon.com/greengrass/v2/APIReference/API_BatchDisassociateClientDeviceWithCoreDevice.html">BatchDisassociateClientDeviceWithCoreDevice</a> operation consumes a list of these requests.
layout: schema
name: DisassociateClientDeviceFromCoreDeviceEntry
properties_list:
- description: ''
  name: thingName
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-disassociate-client-device-from-core-device-entry-schema.json
slug: iot-greengrass-disassociate-client-device-from-core-device-entry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-disassociate-client-device-from-core-device-entry-schema.json\",\n  \"title\": \"DisassociateClientDeviceFromCoreDeviceEntry\",\n  \"description\": \"Contains a request to disassociate a client device from a core device. The <a href=\\\"https://docs.aws.amazon.com/greengrass/v2/APIReference/API_BatchDisassociateClientDeviceWithCoreDevice.html\\\">BatchDisassociateClientDeviceWithCoreDevice</a> operation consumes a list of these requests.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"thingName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IoTThingName\"\n        },\n        {\n          \"description\": \"The name of the IoT thing that represents the client device to disassociate.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n   \
  \ \"thingName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-disassociate-client-device-from-core-device-entry-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: DisassociateClientDeviceFromCoreDeviceEntry
---
