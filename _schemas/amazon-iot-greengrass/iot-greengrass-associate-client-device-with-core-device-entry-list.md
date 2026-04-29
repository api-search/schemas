---
description: AssociateClientDeviceWithCoreDeviceEntryList schema
layout: schema
name: AssociateClientDeviceWithCoreDeviceEntryList
properties_list: []
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-associate-client-device-with-core-device-entry-list-schema.json
slug: iot-greengrass-associate-client-device-with-core-device-entry-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-associate-client-device-with-core-device-entry-list-schema.json\",\n  \"title\": \"AssociateClientDeviceWithCoreDeviceEntryList\",\n  \"description\": \"AssociateClientDeviceWithCoreDeviceEntryList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"thingName\"\n    ],\n    \"properties\": {\n      \"thingName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/IoTThingName\"\n          },\n          {\n            \"description\": \"The name of the IoT thing that represents the client device to associate.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains a request to associate a client device with a core device. The <a href=\\\"https://docs.aws.amazon.com/greengrass/v2/APIReference/API_BatchAssociateClientDeviceWithCoreDevice.html\\\
  \">BatchAssociateClientDeviceWithCoreDevice</a> operation consumes a list of these requests.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-associate-client-device-with-core-device-entry-list-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: AssociateClientDeviceWithCoreDeviceEntryList
---
