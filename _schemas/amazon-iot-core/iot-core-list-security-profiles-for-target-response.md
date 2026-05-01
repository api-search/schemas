---
description: ListSecurityProfilesForTargetResponse schema
layout: schema
name: ListSecurityProfilesForTargetResponse
properties_list:
- description: ''
  name: securityProfileTargetMappings
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-list-security-profiles-for-target-response-schema.json
slug: iot-core-list-security-profiles-for-target-response
source_filename: iot-core-list-security-profiles-for-target-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-security-profiles-for-target-response-schema.json\",\n  \"title\": \"ListSecurityProfilesForTargetResponse\",\n  \"description\": \"ListSecurityProfilesForTargetResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"securityProfileTargetMappings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityProfileTargetMappings\"\n        },\n        {\n          \"description\": \"A list of security profiles and their associated targets.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token that can be used to retrieve the next set of results, or <code>null</code> if there are no additional results.\"\n\
  \        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-security-profiles-for-target-response-schema.json
tags:
- Device Management
- IoT
- MQTT
- Message Routing
title: ListSecurityProfilesForTargetResponse
---
