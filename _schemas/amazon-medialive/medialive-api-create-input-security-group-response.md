---
description: Placeholder documentation for CreateInputSecurityGroupResponse
layout: schema
name: CreateInputSecurityGroupResponse
properties_list:
- description: ''
  name: SecurityGroup
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-create-input-security-group-response-schema.json
slug: medialive-api-create-input-security-group-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-create-input-security-group-response-schema.json\",\n  \"title\": \"CreateInputSecurityGroupResponse\",\n  \"description\": \"Placeholder documentation for CreateInputSecurityGroupResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SecurityGroup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputSecurityGroup\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"securityGroup\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-create-input-security-group-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CreateInputSecurityGroupResponse
---
