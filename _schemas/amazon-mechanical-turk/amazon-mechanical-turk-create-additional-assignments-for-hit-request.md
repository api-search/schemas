---
description: CreateAdditionalAssignmentsForHITRequest schema from Amazon Mechanical Turk API
layout: schema
name: CreateAdditionalAssignmentsForHITRequest
properties_list:
- description: ''
  name: HITId
  type: object
- description: ''
  name: NumberOfAdditionalAssignments
  type: object
- description: ''
  name: UniqueRequestToken
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-create-additional-assignments-for-hit-request-schema.json
slug: amazon-mechanical-turk-create-additional-assignments-for-hit-request
source_filename: amazon-mechanical-turk-create-additional-assignments-for-hit-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-create-additional-assignments-for-hit-request-schema.json\",\n  \"title\": \"CreateAdditionalAssignmentsForHITRequest\",\n  \"description\": \"CreateAdditionalAssignmentsForHITRequest schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HITId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \"The ID of the HIT to extend.\"\n        }\n      ]\n    },\n    \"NumberOfAdditionalAssignments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of additional assignments to request for this HIT.\"\n        }\n      ]\n    },\n    \"UniqueRequestToken\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdempotencyToken\"\n        },\n        {\n          \"description\": \" A unique identifier for this request, which allows you to retry the call on error without extending the HIT multiple times. This is useful in cases such as network timeouts where it is unclear whether or not the call succeeded on the server. If the extend HIT already exists in the system from a previous call using the same <code>UniqueRequestToken</code>, subsequent calls will return an error with a message containing the request ID. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"HITId\",\n    \"NumberOfAdditionalAssignments\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-create-additional-assignments-for-hit-request-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: CreateAdditionalAssignmentsForHITRequest
---
