---
description: GetAssignmentResponse schema from Amazon Mechanical Turk API
layout: schema
name: GetAssignmentResponse
properties_list:
- description: ''
  name: Assignment
  type: object
- description: ''
  name: HIT
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-get-assignment-response-schema.json
slug: amazon-mechanical-turk-get-assignment-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-get-assignment-response-schema.json\",\n  \"title\": \"GetAssignmentResponse\",\n  \"description\": \"GetAssignmentResponse schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Assignment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Assignment\"\n        },\n        {\n          \"description\": \" The assignment. The response includes one Assignment element. \"\n        }\n      ]\n    },\n    \"HIT\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HIT\"\n        },\n        {\n          \"description\": \" The HIT associated with this assignment. The response includes one HIT element.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-get-assignment-response-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: GetAssignmentResponse
---
