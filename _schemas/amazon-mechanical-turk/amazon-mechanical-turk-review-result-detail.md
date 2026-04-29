---
description: This data structure is returned multiple times for each result specified in the Review Policy.
layout: schema
name: ReviewResultDetail
properties_list:
- description: ''
  name: ActionId
  type: object
- description: ''
  name: SubjectId
  type: object
- description: ''
  name: SubjectType
  type: object
- description: ''
  name: QuestionId
  type: object
- description: ''
  name: Key
  type: object
- description: ''
  name: Value
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-review-result-detail-schema.json
slug: amazon-mechanical-turk-review-result-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-review-result-detail-schema.json\",\n  \"title\": \"ReviewResultDetail\",\n  \"description\": \" This data structure is returned multiple times for each result specified in the Review Policy. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ActionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \" A unique identifier of the Review action result. \"\n        }\n      ]\n    },\n    \"SubjectId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \"The HITID or AssignmentId about which this result was taken. Note that HIT-level Review Policies will often emit results about both the HIT\
  \ itself and its Assignments, while Assignment-level review policies generally only emit results about the Assignment itself. \"\n        }\n      ]\n    },\n    \"SubjectType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The type of the object from the SubjectId field.\"\n        }\n      ]\n    },\n    \"QuestionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \" Specifies the QuestionId the result is describing. Depending on whether the TargetType is a HIT or Assignment this results could specify multiple values. If TargetType is HIT and QuestionId is absent, then the result describes results of the HIT, including the HIT agreement score. If ObjectType is Assignment and QuestionId is absent, then the result describes the Worker's performance on the HIT. \"\n        }\n      ]\n    },\n    \"Key\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" Key identifies the particular piece of reviewed information. \"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The values of Key provided by the review policies you have selected. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-review-result-detail-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: ReviewResultDetail
---
