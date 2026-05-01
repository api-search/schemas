---
description: Placeholder documentation for UpdateInputSecurityGroupResponse
layout: schema
name: UpdateInputSecurityGroupResponse
properties_list:
- description: ''
  name: SecurityGroup
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-update-input-security-group-response-schema.json
slug: medialive-api-update-input-security-group-response
source_filename: medialive-api-update-input-security-group-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-update-input-security-group-response-schema.json\",\n  \"title\": \"UpdateInputSecurityGroupResponse\",\n  \"description\": \"Placeholder documentation for UpdateInputSecurityGroupResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SecurityGroup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputSecurityGroup\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"securityGroup\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-update-input-security-group-response-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: UpdateInputSecurityGroupResponse
---
