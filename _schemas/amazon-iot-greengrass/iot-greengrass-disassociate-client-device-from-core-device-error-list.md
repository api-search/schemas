---
description: DisassociateClientDeviceFromCoreDeviceErrorList schema
layout: schema
name: DisassociateClientDeviceFromCoreDeviceErrorList
properties_list: []
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-disassociate-client-device-from-core-device-error-list-schema.json
slug: iot-greengrass-disassociate-client-device-from-core-device-error-list
source_filename: iot-greengrass-disassociate-client-device-from-core-device-error-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-disassociate-client-device-from-core-device-error-list-schema.json\",\n  \"title\": \"DisassociateClientDeviceFromCoreDeviceErrorList\",\n  \"description\": \"DisassociateClientDeviceFromCoreDeviceErrorList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"thingName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/IoTThingName\"\n          },\n          {\n            \"description\": \"The name of the IoT thing whose disassociate request failed.\"\n          }\n        ]\n      },\n      \"code\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/NonEmptyString\"\n          },\n          {\n            \"description\": \"The error code for the request.\"\
  \n          }\n        ]\n      },\n      \"message\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/NonEmptyString\"\n          },\n          {\n            \"description\": \"A message that provides additional information about the error.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains an error that occurs from a request to disassociate a client device from a core device. The <a href=\\\"https://docs.aws.amazon.com/greengrass/v2/APIReference/API_BatchDisassociateClientDeviceWithCoreDevice.html\\\">BatchDisassociateClientDeviceWithCoreDevice</a> operation returns a list of these errors.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-disassociate-client-device-from-core-device-error-list-schema.json
tags:
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: DisassociateClientDeviceFromCoreDeviceErrorList
---
