---
description: RejectAssignmentRequest schema from Amazon Mechanical Turk API
layout: schema
name: RejectAssignmentRequest
properties_list:
- description: ''
  name: AssignmentId
  type: object
- description: ''
  name: RequesterFeedback
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-reject-assignment-request-schema.json
slug: amazon-mechanical-turk-reject-assignment-request
source_filename: amazon-mechanical-turk-reject-assignment-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-reject-assignment-request-schema.json\",\n  \"title\": \"RejectAssignmentRequest\",\n  \"description\": \"RejectAssignmentRequest schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AssignmentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \" The ID of the assignment. The assignment must correspond to a HIT created by the Requester. \"\n        }\n      ]\n    },\n    \"RequesterFeedback\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" A message for the Worker, which the Worker can see in the Status section of the web site. \"\n        }\n   \
  \   ]\n    }\n  },\n  \"required\": [\n    \"AssignmentId\",\n    \"RequesterFeedback\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-reject-assignment-request-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: RejectAssignmentRequest
---
