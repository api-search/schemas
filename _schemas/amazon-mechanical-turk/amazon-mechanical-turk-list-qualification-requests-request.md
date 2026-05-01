---
description: ListQualificationRequestsRequest schema from Amazon Mechanical Turk API
layout: schema
name: ListQualificationRequestsRequest
properties_list:
- description: ''
  name: QualificationTypeId
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-list-qualification-requests-request-schema.json
slug: amazon-mechanical-turk-list-qualification-requests-request
source_filename: amazon-mechanical-turk-list-qualification-requests-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-list-qualification-requests-request-schema.json\",\n  \"title\": \"ListQualificationRequestsRequest\",\n  \"description\": \"ListQualificationRequestsRequest schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"QualificationTypeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \"The ID of the QualificationType.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/PaginationToken\"\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResultSize\"\n        },\n        {\n          \"description\": \" The maximum number of results to return in a single\
  \ call. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-list-qualification-requests-request-schema.json
tags:
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: ListQualificationRequestsRequest
---
