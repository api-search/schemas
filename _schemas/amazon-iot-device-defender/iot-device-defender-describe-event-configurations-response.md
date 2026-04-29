---
description: DescribeEventConfigurationsResponse schema
layout: schema
name: DescribeEventConfigurationsResponse
properties_list:
- description: ''
  name: eventConfigurations
  type: object
- description: ''
  name: creationDate
  type: object
- description: ''
  name: lastModifiedDate
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-describe-event-configurations-response-schema.json
slug: iot-device-defender-describe-event-configurations-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-describe-event-configurations-response-schema.json\",\n  \"title\": \"DescribeEventConfigurationsResponse\",\n  \"description\": \"DescribeEventConfigurationsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventConfigurations\"\n        },\n        {\n          \"description\": \"The event configurations.\"\n        }\n      ]\n    },\n    \"creationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreationDate\"\n        },\n        {\n          \"description\": \"The creation date of the event configuration.\"\n        }\n      ]\n    },\n    \"lastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/LastModifiedDate\"\n        },\n        {\n          \"description\": \"The date the event configurations were last modified.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-describe-event-configurations-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: DescribeEventConfigurationsResponse
---
