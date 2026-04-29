---
description: ListReviewPolicyResultsForHITResponse schema from Amazon Mechanical Turk API
layout: schema
name: ListReviewPolicyResultsForHITResponse
properties_list:
- description: ''
  name: HITId
  type: object
- description: ''
  name: AssignmentReviewPolicy
  type: object
- description: ''
  name: HITReviewPolicy
  type: object
- description: ''
  name: AssignmentReviewReport
  type: object
- description: ''
  name: HITReviewReport
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-list-review-policy-results-for-hit-response-schema.json
slug: amazon-mechanical-turk-list-review-policy-results-for-hit-response
source_filename: amazon-mechanical-turk-list-review-policy-results-for-hit-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-list-review-policy-results-for-hit-response-schema.json\",\n  \"title\": \"ListReviewPolicyResultsForHITResponse\",\n  \"description\": \"ListReviewPolicyResultsForHITResponse schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HITId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \"The HITId of the HIT for which results have been returned.\"\n        }\n      ]\n    },\n    \"AssignmentReviewPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReviewPolicy\"\n        },\n        {\n          \"description\": \" The name of the Assignment-level Review Policy. This contains only the PolicyName element. \"\n\
  \        }\n      ]\n    },\n    \"HITReviewPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReviewPolicy\"\n        },\n        {\n          \"description\": \"The name of the HIT-level Review Policy. This contains only the PolicyName element.\"\n        }\n      ]\n    },\n    \"AssignmentReviewReport\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReviewReport\"\n        },\n        {\n          \"description\": \" Contains both ReviewResult and ReviewAction elements for an Assignment. \"\n        }\n      ]\n    },\n    \"HITReviewReport\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReviewReport\"\n        },\n        {\n          \"description\": \"Contains both ReviewResult and ReviewAction elements for a particular HIT. \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/PaginationToken\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-list-review-policy-results-for-hit-response-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: ListReviewPolicyResultsForHITResponse
---
