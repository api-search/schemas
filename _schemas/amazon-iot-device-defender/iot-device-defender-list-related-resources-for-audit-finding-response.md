---
description: ListRelatedResourcesForAuditFindingResponse schema
layout: schema
name: ListRelatedResourcesForAuditFindingResponse
properties_list:
- description: ''
  name: relatedResources
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-list-related-resources-for-audit-finding-response-schema.json
slug: iot-device-defender-list-related-resources-for-audit-finding-response
source_filename: iot-device-defender-list-related-resources-for-audit-finding-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-list-related-resources-for-audit-finding-response-schema.json\",\n  \"title\": \"ListRelatedResourcesForAuditFindingResponse\",\n  \"description\": \"ListRelatedResourcesForAuditFindingResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"relatedResources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RelatedResources\"\n        },\n        {\n          \"description\": \"The related resources.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token that can be used to retrieve the next set of results, or <code>null</code> for the first API call.\"\n        }\n      ]\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-list-related-resources-for-audit-finding-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: ListRelatedResourcesForAuditFindingResponse
---
