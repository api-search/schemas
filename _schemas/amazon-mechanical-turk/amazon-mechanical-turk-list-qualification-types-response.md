---
description: ListQualificationTypesResponse schema from Amazon Mechanical Turk API
layout: schema
name: ListQualificationTypesResponse
properties_list:
- description: ''
  name: NumResults
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: QualificationTypes
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-list-qualification-types-response-schema.json
slug: amazon-mechanical-turk-list-qualification-types-response
source_filename: amazon-mechanical-turk-list-qualification-types-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-list-qualification-types-response-schema.json\",\n  \"title\": \"ListQualificationTypesResponse\",\n  \"description\": \"ListQualificationTypesResponse schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NumResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \" The number of Qualification types on this page in the filtered results list, equivalent to the number of types this operation returns. \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/PaginationToken\"\n    },\n    \"QualificationTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QualificationTypeList\"\
  \n        },\n        {\n          \"description\": \" The list of QualificationType elements returned by the query. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-list-qualification-types-response-schema.json
tags:
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: ListQualificationTypesResponse
---
