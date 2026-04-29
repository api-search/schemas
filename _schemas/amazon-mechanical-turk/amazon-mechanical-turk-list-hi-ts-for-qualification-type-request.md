---
description: ListHITsForQualificationTypeRequest schema from Amazon Mechanical Turk API
layout: schema
name: ListHITsForQualificationTypeRequest
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
schema_file: json-schema/amazon-mechanical-turk-list-hi-ts-for-qualification-type-request-schema.json
slug: amazon-mechanical-turk-list-hi-ts-for-qualification-type-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-list-hi-ts-for-qualification-type-request-schema.json\",\n  \"title\": \"ListHITsForQualificationTypeRequest\",\n  \"description\": \"ListHITsForQualificationTypeRequest schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"QualificationTypeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \" The ID of the Qualification type to use when querying HITs. \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"Pagination Token\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n  \
  \      {\n          \"$ref\": \"#/components/schemas/ResultSize\"\n        },\n        {\n          \"description\": \" Limit the number of results returned. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"QualificationTypeId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-list-hi-ts-for-qualification-type-request-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: ListHITsForQualificationTypeRequest
---
