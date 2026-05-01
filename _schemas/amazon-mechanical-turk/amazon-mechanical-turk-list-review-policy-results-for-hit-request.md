---
description: ListReviewPolicyResultsForHITRequest schema from Amazon Mechanical Turk API
layout: schema
name: ListReviewPolicyResultsForHITRequest
properties_list:
- description: ''
  name: HITId
  type: object
- description: ''
  name: PolicyLevels
  type: object
- description: ''
  name: RetrieveActions
  type: object
- description: ''
  name: RetrieveResults
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-list-review-policy-results-for-hit-request-schema.json
slug: amazon-mechanical-turk-list-review-policy-results-for-hit-request
source_filename: amazon-mechanical-turk-list-review-policy-results-for-hit-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-list-review-policy-results-for-hit-request-schema.json\",\n  \"title\": \"ListReviewPolicyResultsForHITRequest\",\n  \"description\": \"ListReviewPolicyResultsForHITRequest schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HITId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \"The unique identifier of the HIT to retrieve review results for.\"\n        }\n      ]\n    },\n    \"PolicyLevels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReviewPolicyLevelList\"\n        },\n        {\n          \"description\": \" The Policy Level(s) to retrieve review results for - HIT or Assignment. If omitted, the default\
  \ behavior is to retrieve all data for both policy levels. For a list of all the described policies, see Review Policies. \"\n        }\n      ]\n    },\n    \"RetrieveActions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \" Specify if the operation should retrieve a list of the actions taken executing the Review Policies and their outcomes. \"\n        }\n      ]\n    },\n    \"RetrieveResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \" Specify if the operation should retrieve a list of the results computed by the Review Policies. \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"Pagination token\"\n        }\n      ]\n    },\n    \"MaxResults\":\
  \ {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResultSize\"\n        },\n        {\n          \"description\": \"Limit the number of results returned.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"HITId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-list-review-policy-results-for-hit-request-schema.json
tags:
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: ListReviewPolicyResultsForHITRequest
---
