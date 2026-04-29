---
description: AssociateQualificationWithWorkerRequest schema from Amazon Mechanical Turk API
layout: schema
name: AssociateQualificationWithWorkerRequest
properties_list:
- description: ''
  name: QualificationTypeId
  type: object
- description: ''
  name: WorkerId
  type: object
- description: ''
  name: IntegerValue
  type: object
- description: ''
  name: SendNotification
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-associate-qualification-with-worker-request-schema.json
slug: amazon-mechanical-turk-associate-qualification-with-worker-request
source_filename: amazon-mechanical-turk-associate-qualification-with-worker-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-associate-qualification-with-worker-request-schema.json\",\n  \"title\": \"AssociateQualificationWithWorkerRequest\",\n  \"description\": \"AssociateQualificationWithWorkerRequest schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"QualificationTypeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \"The ID of the Qualification type to use for the assigned Qualification.\"\n        }\n      ]\n    },\n    \"WorkerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomerId\"\n        },\n        {\n          \"description\": \" The ID of the Worker to whom the Qualification is being assigned. Worker IDs are\
  \ included with submitted HIT assignments and Qualification requests. \"\n        }\n      ]\n    },\n    \"IntegerValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The value of the Qualification to assign.\"\n        }\n      ]\n    },\n    \"SendNotification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \" Specifies whether to send a notification email message to the Worker saying that the qualification was assigned to the Worker. Note: this is true by default. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"QualificationTypeId\",\n    \"WorkerId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-associate-qualification-with-worker-request-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: AssociateQualificationWithWorkerRequest
---
