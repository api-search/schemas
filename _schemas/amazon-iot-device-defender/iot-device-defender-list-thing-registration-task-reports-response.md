---
description: ListThingRegistrationTaskReportsResponse schema
layout: schema
name: ListThingRegistrationTaskReportsResponse
properties_list:
- description: ''
  name: resourceLinks
  type: object
- description: ''
  name: reportType
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-list-thing-registration-task-reports-response-schema.json
slug: iot-device-defender-list-thing-registration-task-reports-response
source_filename: iot-device-defender-list-thing-registration-task-reports-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-list-thing-registration-task-reports-response-schema.json\",\n  \"title\": \"ListThingRegistrationTaskReportsResponse\",\n  \"description\": \"ListThingRegistrationTaskReportsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceLinks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3FileUrlList\"\n        },\n        {\n          \"description\": \"Links to the task resources.\"\n        }\n      ]\n    },\n    \"reportType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportType\"\n        },\n        {\n          \"description\": \"The type of task report.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\
  \n        },\n        {\n          \"description\": \"The token to use to get the next set of results, or <b>null</b> if there are no additional results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-list-thing-registration-task-reports-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: ListThingRegistrationTaskReportsResponse
---
