---
description: ListReviewableHITsRequest schema from Amazon Mechanical Turk API
layout: schema
name: ListReviewableHITsRequest
properties_list:
- description: ''
  name: HITTypeId
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-list-reviewable-hi-ts-request-schema.json
slug: amazon-mechanical-turk-list-reviewable-hi-ts-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-list-reviewable-hi-ts-request-schema.json\",\n  \"title\": \"ListReviewableHITsRequest\",\n  \"description\": \"ListReviewableHITsRequest schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HITTypeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \" The ID of the HIT type of the HITs to consider for the query. If not specified, all HITs for the Reviewer are considered \"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReviewableHITStatus\"\n        },\n        {\n          \"description\": \" Can be either <code>Reviewable</code> or <code>Reviewing</code>. Reviewable\
  \ is the default value. \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"Pagination Token\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResultSize\"\n        },\n        {\n          \"description\": \" Limit the number of results returned. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-list-reviewable-hi-ts-request-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: ListReviewableHITsRequest
---
