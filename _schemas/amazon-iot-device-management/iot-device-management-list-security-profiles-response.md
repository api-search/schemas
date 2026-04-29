---
description: ListSecurityProfilesResponse schema
layout: schema
name: ListSecurityProfilesResponse
properties_list:
- description: ''
  name: securityProfileIdentifiers
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-list-security-profiles-response-schema.json
slug: iot-device-management-list-security-profiles-response
source_filename: iot-device-management-list-security-profiles-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-security-profiles-response-schema.json\",\n  \"title\": \"ListSecurityProfilesResponse\",\n  \"description\": \"ListSecurityProfilesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"securityProfileIdentifiers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityProfileIdentifiers\"\n        },\n        {\n          \"description\": \"A list of security profile identifiers (names and ARNs).\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token that can be used to retrieve the next set of results, or <code>null</code> if there are no additional results.\"\n        }\n\
  \      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-security-profiles-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: ListSecurityProfilesResponse
---
