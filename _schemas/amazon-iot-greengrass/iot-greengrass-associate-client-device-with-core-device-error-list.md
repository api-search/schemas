---
description: AssociateClientDeviceWithCoreDeviceErrorList schema
layout: schema
name: AssociateClientDeviceWithCoreDeviceErrorList
properties_list: []
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-associate-client-device-with-core-device-error-list-schema.json
slug: iot-greengrass-associate-client-device-with-core-device-error-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-associate-client-device-with-core-device-error-list-schema.json\",\n  \"title\": \"AssociateClientDeviceWithCoreDeviceErrorList\",\n  \"description\": \"AssociateClientDeviceWithCoreDeviceErrorList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"thingName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/IoTThingName\"\n          },\n          {\n            \"description\": \"The name of the IoT thing whose associate request failed.\"\n          }\n        ]\n      },\n      \"code\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/NonEmptyString\"\n          },\n          {\n            \"description\": \"The error code for the request.\"\n         \
  \ }\n        ]\n      },\n      \"message\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/NonEmptyString\"\n          },\n          {\n            \"description\": \"A message that provides additional information about the error.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains an error that occurs from a request to associate a client device with a core device. The <a href=\\\"https://docs.aws.amazon.com/greengrass/v2/APIReference/API_BatchAssociateClientDeviceWithCoreDevice.html\\\">BatchAssociateClientDeviceWithCoreDevice</a> operation returns a list of these errors.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-associate-client-device-with-core-device-error-list-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: AssociateClientDeviceWithCoreDeviceErrorList
---
