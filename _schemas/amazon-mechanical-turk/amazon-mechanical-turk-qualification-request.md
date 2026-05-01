---
description: The QualificationRequest data structure represents a request a Worker has made for a Qualification.
layout: schema
name: QualificationRequest
properties_list:
- description: ''
  name: QualificationRequestId
  type: object
- description: ''
  name: QualificationTypeId
  type: object
- description: ''
  name: WorkerId
  type: object
- description: ''
  name: Test
  type: object
- description: ''
  name: Answer
  type: object
- description: ''
  name: SubmitTime
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-qualification-request-schema.json
slug: amazon-mechanical-turk-qualification-request
source_filename: amazon-mechanical-turk-qualification-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-qualification-request-schema.json\",\n  \"title\": \"QualificationRequest\",\n  \"description\": \" The QualificationRequest data structure represents a request a Worker has made for a Qualification. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"QualificationRequestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The ID of the Qualification request, a unique identifier generated when the request was submitted. \"\n        }\n      ]\n    },\n    \"QualificationTypeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \" The ID of the Qualification type the Worker is requesting,\
  \ as returned by the CreateQualificationType operation. \"\n        }\n      ]\n    },\n    \"WorkerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomerId\"\n        },\n        {\n          \"description\": \" The ID of the Worker requesting the Qualification.\"\n        }\n      ]\n    },\n    \"Test\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The contents of the Qualification test that was presented to the Worker, if the type has a test and the Worker has submitted answers. This value is identical to the QuestionForm associated with the Qualification type at the time the Worker requests the Qualification.\"\n        }\n      ]\n    },\n    \"Answer\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The Worker's answers for the Qualification type's test contained\
  \ in a QuestionFormAnswers document, if the type has a test and the Worker has submitted answers. If the Worker does not provide any answers, Answer may be empty. \"\n        }\n      ]\n    },\n    \"SubmitTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time the Qualification request had a status of Submitted. This is either the time the Worker submitted answers for a Qualification test, or the time the Worker requested the Qualification if the Qualification type does not have a test. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-qualification-request-schema.json
tags:
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: QualificationRequest
---
