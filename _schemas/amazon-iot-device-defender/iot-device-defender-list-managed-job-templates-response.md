---
description: ListManagedJobTemplatesResponse schema
layout: schema
name: ListManagedJobTemplatesResponse
properties_list:
- description: ''
  name: managedJobTemplates
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-list-managed-job-templates-response-schema.json
slug: iot-device-defender-list-managed-job-templates-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-list-managed-job-templates-response-schema.json\",\n  \"title\": \"ListManagedJobTemplatesResponse\",\n  \"description\": \"ListManagedJobTemplatesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"managedJobTemplates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ManagedJobTemplatesSummaryList\"\n        },\n        {\n          \"description\": \"A list of managed job templates that are returned.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token to retrieve the next set of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-list-managed-job-templates-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: ListManagedJobTemplatesResponse
---
