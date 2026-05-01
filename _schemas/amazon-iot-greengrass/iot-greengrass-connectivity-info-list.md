---
description: connectivityInfoList schema
layout: schema
name: connectivityInfoList
properties_list: []
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-connectivity-info-list-schema.json
slug: iot-greengrass-connectivity-info-list
source_filename: iot-greengrass-connectivity-info-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-connectivity-info-list-schema.json\",\n  \"title\": \"connectivityInfoList\",\n  \"description\": \"connectivityInfoList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"id\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/String\"\n          },\n          {\n            \"xml\": {\n              \"name\": \"Id\"\n            },\n            \"description\": \"An ID for the connectivity information.\"\n          }\n        ]\n      },\n      \"hostAddress\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/String\"\n          },\n          {\n            \"xml\": {\n              \"name\": \"HostAddress\"\n            },\n            \"description\": \"\
  The IP address or DNS address where client devices can connect to an MQTT broker on the Greengrass core device.\"\n          }\n        ]\n      },\n      \"portNumber\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/PortNumberInt\"\n          },\n          {\n            \"xml\": {\n              \"name\": \"PortNumber\"\n            },\n            \"description\": \"The port where the MQTT broker operates on the core device. This port is typically 8883, which is the default port for the MQTT broker component that runs on core devices.\"\n          }\n        ]\n      },\n      \"metadata\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/String\"\n          },\n          {\n            \"xml\": {\n              \"name\": \"Metadata\"\n            },\n            \"description\": \"Additional metadata to provide to client devices that connect to this core device.\"\n          }\n        ]\n      }\n    },\n    \"\
  description\": \"Contains information about an endpoint and port where client devices can connect to an MQTT broker on a Greengrass core device.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-connectivity-info-list-schema.json
tags:
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: connectivityInfoList
---
