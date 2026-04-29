---
description: UpdateQualificationTypeRequest schema from Amazon Mechanical Turk API
layout: schema
name: UpdateQualificationTypeRequest
properties_list:
- description: ''
  name: QualificationTypeId
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: QualificationTypeStatus
  type: object
- description: ''
  name: Test
  type: object
- description: ''
  name: AnswerKey
  type: object
- description: ''
  name: TestDurationInSeconds
  type: object
- description: ''
  name: RetryDelayInSeconds
  type: object
- description: ''
  name: AutoGranted
  type: object
- description: ''
  name: AutoGrantedValue
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-update-qualification-type-request-schema.json
slug: amazon-mechanical-turk-update-qualification-type-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-update-qualification-type-request-schema.json\",\n  \"title\": \"UpdateQualificationTypeRequest\",\n  \"description\": \"UpdateQualificationTypeRequest schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"QualificationTypeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \"The ID of the Qualification type to update.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The new description of the Qualification type.\"\n        }\n      ]\n    },\n    \"QualificationTypeStatus\": {\n      \"allOf\": [\n  \
  \      {\n          \"$ref\": \"#/components/schemas/QualificationTypeStatus\"\n        },\n        {\n          \"description\": \"The new status of the Qualification type - Active | Inactive\"\n        }\n      ]\n    },\n    \"Test\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>The questions for the Qualification test a Worker must answer correctly to obtain a Qualification of this type. If this parameter is specified, <code>TestDurationInSeconds</code> must also be specified.</p> <p>Constraints: Must not be longer than 65535 bytes. Must be a QuestionForm data structure. This parameter cannot be specified if AutoGranted is true.</p> <p>Constraints: None. If not specified, the Worker may request the Qualification without answering any questions.</p>\"\n        }\n      ]\n    },\n    \"AnswerKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n  \
  \      },\n        {\n          \"description\": \"The answers to the Qualification test specified in the Test parameter, in the form of an AnswerKey data structure.\"\n        }\n      ]\n    },\n    \"TestDurationInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The number of seconds the Worker has to complete the Qualification test, starting from the time the Worker requests the Qualification.\"\n        }\n      ]\n    },\n    \"RetryDelayInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The amount of time, in seconds, that Workers must wait after requesting a Qualification of the specified Qualification type before they can retry the Qualification request. It is not possible to disable retries for a Qualification type after it has been created with retries enabled. If you want to disable\
  \ retries, you must dispose of the existing retry-enabled Qualification type using DisposeQualificationType and then create a new Qualification type with retries disabled using CreateQualificationType.\"\n        }\n      ]\n    },\n    \"AutoGranted\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>Specifies whether requests for the Qualification type are granted immediately, without prompting the Worker with a Qualification test.</p> <p>Constraints: If the Test parameter is specified, this parameter cannot be true.</p>\"\n        }\n      ]\n    },\n    \"AutoGrantedValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The Qualification value to use for automatically granted Qualifications. This parameter is used only if the AutoGranted parameter is true.\"\n        }\n      ]\n    }\n  },\n  \"\
  required\": [\n    \"QualificationTypeId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-update-qualification-type-request-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: UpdateQualificationTypeRequest
---
