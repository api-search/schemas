---
description: ListJobTemplatesResponse schema
layout: schema
name: ListJobTemplatesResponse
properties_list:
- description: ''
  name: jobTemplates
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-list-job-templates-response-schema.json
slug: iot-device-management-list-job-templates-response
source_filename: iot-device-management-list-job-templates-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-job-templates-response-schema.json\",\n  \"title\": \"ListJobTemplatesResponse\",\n  \"description\": \"ListJobTemplatesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobTemplates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobTemplateSummaryList\"\n        },\n        {\n          \"description\": \"A list of objects that contain information about the job templates.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token for the next set of results, or <b>null</b> if there are no additional results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-job-templates-response-schema.json
tags:
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: ListJobTemplatesResponse
---
