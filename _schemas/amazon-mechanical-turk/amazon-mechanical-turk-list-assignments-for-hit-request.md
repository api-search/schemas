---
description: ListAssignmentsForHITRequest schema from Amazon Mechanical Turk API
layout: schema
name: ListAssignmentsForHITRequest
properties_list:
- description: ''
  name: HITId
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: AssignmentStatuses
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-list-assignments-for-hit-request-schema.json
slug: amazon-mechanical-turk-list-assignments-for-hit-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-list-assignments-for-hit-request-schema.json\",\n  \"title\": \"ListAssignmentsForHITRequest\",\n  \"description\": \"ListAssignmentsForHITRequest schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HITId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \"The ID of the HIT.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"Pagination token\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"$ref\": \"#/components/schemas/ResultSize\"\n    },\n    \"AssignmentStatuses\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/AssignmentStatusList\"\n        },\n        {\n          \"description\": \"The status of the assignments to return: Submitted | Approved | Rejected\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"HITId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-list-assignments-for-hit-request-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: ListAssignmentsForHITRequest
---
