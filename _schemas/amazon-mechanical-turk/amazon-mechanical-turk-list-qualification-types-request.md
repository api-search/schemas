---
description: ListQualificationTypesRequest schema from Amazon Mechanical Turk API
layout: schema
name: ListQualificationTypesRequest
properties_list:
- description: ''
  name: Query
  type: object
- description: ''
  name: MustBeRequestable
  type: object
- description: ''
  name: MustBeOwnedByCaller
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-list-qualification-types-request-schema.json
slug: amazon-mechanical-turk-list-qualification-types-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-list-qualification-types-request-schema.json\",\n  \"title\": \"ListQualificationTypesRequest\",\n  \"description\": \"ListQualificationTypesRequest schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Query\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" A text query against all of the searchable attributes of Qualification types. \"\n        }\n      ]\n    },\n    \"MustBeRequestable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Specifies that only Qualification types that a user can request through the Amazon Mechanical Turk web site, such\
  \ as by taking a Qualification test, are returned as results of the search. Some Qualification types, such as those assigned automatically by the system, cannot be requested directly by users. If false, all Qualification types, including those managed by the system, are considered. Valid values are True | False. \"\n        }\n      ]\n    },\n    \"MustBeOwnedByCaller\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \" Specifies that only Qualification types that the Requester created are returned. If false, the operation returns all Qualification types. \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/PaginationToken\"\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResultSize\"\n        },\n        {\n          \"description\": \" The maximum number of results to return in a single call. \"\n\
  \        }\n      ]\n    }\n  },\n  \"required\": [\n    \"MustBeRequestable\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-list-qualification-types-request-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: ListQualificationTypesRequest
---
