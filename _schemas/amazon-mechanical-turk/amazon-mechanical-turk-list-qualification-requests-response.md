---
description: ListQualificationRequestsResponse schema from Amazon Mechanical Turk API
layout: schema
name: ListQualificationRequestsResponse
properties_list:
- description: ''
  name: NumResults
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: QualificationRequests
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-list-qualification-requests-response-schema.json
slug: amazon-mechanical-turk-list-qualification-requests-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-list-qualification-requests-response-schema.json\",\n  \"title\": \"ListQualificationRequestsResponse\",\n  \"description\": \"ListQualificationRequestsResponse schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NumResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of Qualification requests on this page in the filtered results list, equivalent to the number of Qualification requests being returned by this call.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/PaginationToken\"\n    },\n    \"QualificationRequests\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QualificationRequestList\"\
  \n        },\n        {\n          \"description\": \"The Qualification request. The response includes one QualificationRequest element for each Qualification request returned by the query.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-list-qualification-requests-response-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: ListQualificationRequestsResponse
---
