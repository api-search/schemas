---
description: GetAssignmentRequest schema from Amazon Mechanical Turk API
layout: schema
name: GetAssignmentRequest
properties_list:
- description: ''
  name: AssignmentId
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-get-assignment-request-schema.json
slug: amazon-mechanical-turk-get-assignment-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-get-assignment-request-schema.json\",\n  \"title\": \"GetAssignmentRequest\",\n  \"description\": \"GetAssignmentRequest schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AssignmentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \"The ID of the Assignment to be retrieved.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AssignmentId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-get-assignment-request-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: GetAssignmentRequest
---
