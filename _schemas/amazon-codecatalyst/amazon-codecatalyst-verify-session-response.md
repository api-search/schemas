---
description: VerifySessionResponse schema from Amazon CodeCatalyst
layout: schema
name: VerifySessionResponse
properties_list:
- description: ''
  name: identity
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-verify-session-response-schema.json
slug: amazon-codecatalyst-verify-session-response
source_filename: amazon-codecatalyst-verify-session-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-verify-session-response-schema.json\",\n  \"title\": \"VerifySessionResponse\",\n  \"description\": \"VerifySessionResponse schema from Amazon CodeCatalyst\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"identity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VerifySessionResponseIdentityString\"\n        },\n        {\n          \"description\": \"The system-generated unique ID of the user in Amazon CodeCatalyst.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-verify-session-response-schema.json
tags:
- Amazon
- AWS
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: VerifySessionResponse
---
