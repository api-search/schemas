---
description: Contains the details of an IoT SiteWise error.
layout: schema
name: ErrorDetails
properties_list:
- description: ''
  name: code
  type: object
- description: ''
  name: message
  type: object
- description: ''
  name: details
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-error-details-schema.json
slug: iot-sitewise-error-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-error-details-schema.json\",\n  \"title\": \"ErrorDetails\",\n  \"description\": \"Contains the details of an IoT SiteWise error.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorCode\"\n        },\n        {\n          \"description\": \"The error code.\"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorMessage\"\n        },\n        {\n          \"description\": \"The error message.\"\n        }\n      ]\n    },\n    \"details\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetailedErrors\"\n        },\n        {\n          \"description\": \" A list of detailed errors. \"\n    \
  \    }\n      ]\n    }\n  },\n  \"required\": [\n    \"code\",\n    \"message\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-error-details-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: ErrorDetails
---
