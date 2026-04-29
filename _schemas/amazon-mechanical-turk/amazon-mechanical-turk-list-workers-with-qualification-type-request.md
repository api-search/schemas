---
description: ListWorkersWithQualificationTypeRequest schema from Amazon Mechanical Turk API
layout: schema
name: ListWorkersWithQualificationTypeRequest
properties_list:
- description: ''
  name: QualificationTypeId
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
schema_file: json-schema/amazon-mechanical-turk-list-workers-with-qualification-type-request-schema.json
slug: amazon-mechanical-turk-list-workers-with-qualification-type-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-list-workers-with-qualification-type-request-schema.json\",\n  \"title\": \"ListWorkersWithQualificationTypeRequest\",\n  \"description\": \"ListWorkersWithQualificationTypeRequest schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"QualificationTypeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \"The ID of the Qualification type of the Qualifications to return.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QualificationStatus\"\n        },\n        {\n          \"description\": \" The status of the Qualifications to return. Can be <code>Granted | Revoked</code>.\
  \ \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"Pagination Token\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResultSize\"\n        },\n        {\n          \"description\": \" Limit the number of results returned. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"QualificationTypeId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-list-workers-with-qualification-type-request-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: ListWorkersWithQualificationTypeRequest
---
