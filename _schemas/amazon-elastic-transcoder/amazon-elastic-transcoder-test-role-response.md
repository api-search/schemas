---
description: The <code>TestRoleResponse</code> structure.
layout: schema
name: TestRoleResponse
properties_list:
- description: ''
  name: Success
  type: object
- description: ''
  name: Messages
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-test-role-response-schema.json
slug: amazon-elastic-transcoder-test-role-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-test-role-response-schema.json\",\n  \"title\": \"TestRoleResponse\",\n  \"description\": \"The <code>TestRoleResponse</code> structure.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Success\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Success\"\n        },\n        {\n          \"description\": \"If the operation is successful, this value is <code>true</code>; otherwise, the value is <code>false</code>.\"\n        }\n      ]\n    },\n    \"Messages\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExceptionMessages\"\n        },\n        {\n          \"description\": \"If the <code>Success</code> element contains <code>false</code>, this value is an array of one or more error messages that were\
  \ generated during the test process.\"\n        }\n      ]\n    }\n  },\n  \"deprecated\": true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-test-role-response-schema.json
tags:
- Amazon Web Services
- AWS
- Media
- Transcoding
- Video
title: TestRoleResponse
---
