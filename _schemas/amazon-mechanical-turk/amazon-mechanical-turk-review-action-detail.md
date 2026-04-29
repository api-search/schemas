---
description: Both the AssignmentReviewReport and the HITReviewReport elements contains the ReviewActionDetail data structure. This structure is returned multiple times for each action specified in the Review Policy.
layout: schema
name: ReviewActionDetail
properties_list:
- description: ''
  name: ActionId
  type: object
- description: ''
  name: ActionName
  type: object
- description: ''
  name: TargetId
  type: object
- description: ''
  name: TargetType
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: CompleteTime
  type: object
- description: ''
  name: Result
  type: object
- description: ''
  name: ErrorCode
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-review-action-detail-schema.json
slug: amazon-mechanical-turk-review-action-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-review-action-detail-schema.json\",\n  \"title\": \"ReviewActionDetail\",\n  \"description\": \" Both the AssignmentReviewReport and the HITReviewReport elements contains the ReviewActionDetail data structure. This structure is returned multiple times for each action specified in the Review Policy. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ActionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \"The unique identifier for the action.\"\n        }\n      ]\n    },\n    \"ActionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The nature of the action itself. The Review\
  \ Policy is responsible for examining the HIT and Assignments, emitting results, and deciding which other actions will be necessary. \"\n        }\n      ]\n    },\n    \"TargetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \" The specific HITId or AssignmentID targeted by the action.\"\n        }\n      ]\n    },\n    \"TargetType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The type of object in TargetId.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReviewActionStatus\"\n        },\n        {\n          \"description\": \" The current disposition of the action: INTENDED, SUCCEEDED, FAILED, or CANCELLED. \"\n        }\n      ]\n    },\n    \"CompleteTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\
  \n        },\n        {\n          \"description\": \" The date when the action was completed.\"\n        }\n      ]\n    },\n    \"Result\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" A description of the outcome of the review.\"\n        }\n      ]\n    },\n    \"ErrorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" Present only when the Results have a FAILED Status.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-review-action-detail-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: ReviewActionDetail
---
