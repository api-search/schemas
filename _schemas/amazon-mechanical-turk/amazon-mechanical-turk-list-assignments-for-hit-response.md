---
description: ListAssignmentsForHITResponse schema from Amazon Mechanical Turk API
layout: schema
name: ListAssignmentsForHITResponse
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: NumResults
  type: object
- description: ''
  name: Assignments
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-list-assignments-for-hit-response-schema.json
slug: amazon-mechanical-turk-list-assignments-for-hit-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-list-assignments-for-hit-response-schema.json\",\n  \"title\": \"ListAssignmentsForHITResponse\",\n  \"description\": \"ListAssignmentsForHITResponse schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/PaginationToken\"\n    },\n    \"NumResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \" The number of assignments on the page in the filtered results list, equivalent to the number of assignments returned by this call.\"\n        }\n      ]\n    },\n    \"Assignments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssignmentList\"\n        },\n    \
  \    {\n          \"description\": \" The collection of Assignment data structures returned by this call.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-list-assignments-for-hit-response-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: ListAssignmentsForHITResponse
---
