---
description: The QualificationType data structure represents a Qualification type, a description of a property of a Worker that must match the requirements of a HIT for the Worker to be able to accept the HIT. The type also describes how a Worker can obtain a Qualification of that type, such as through a Qualification test.
layout: schema
name: QualificationType
properties_list:
- description: ''
  name: QualificationTypeId
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Keywords
  type: object
- description: ''
  name: QualificationTypeStatus
  type: object
- description: ''
  name: Test
  type: object
- description: ''
  name: TestDurationInSeconds
  type: object
- description: ''
  name: AnswerKey
  type: object
- description: ''
  name: RetryDelayInSeconds
  type: object
- description: ''
  name: IsRequestable
  type: object
- description: ''
  name: AutoGranted
  type: object
- description: ''
  name: AutoGrantedValue
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-qualification-type-schema.json
slug: amazon-mechanical-turk-qualification-type
source_filename: amazon-mechanical-turk-qualification-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-qualification-type-schema.json\",\n  \"title\": \"QualificationType\",\n  \"description\": \" The QualificationType data structure represents a Qualification type, a description of a property of a Worker that must match the requirements of a HIT for the Worker to be able to accept the HIT. The type also describes how a Worker can obtain a Qualification of that type, such as through a Qualification test. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"QualificationTypeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \" A unique identifier for the Qualification type. A Qualification type is given a Qualification type ID when you call the CreateQualificationType operation.\
  \ \"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" The date and time the Qualification type was created. \"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The name of the Qualification type. The type name is used to identify the type, and to find the type using a Qualification type search. \"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" A long description for the Qualification type. \"\n        }\n      ]\n    },\n    \"Keywords\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\"\
  : \" One or more words or phrases that describe theQualification type, separated by commas. The Keywords make the type easier to find using a search. \"\n        }\n      ]\n    },\n    \"QualificationTypeStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QualificationTypeStatus\"\n        },\n        {\n          \"description\": \" The status of the Qualification type. A Qualification type's status determines if users can apply to receive a Qualification of this type, and if HITs can be created with requirements based on this type. Valid values are Active | Inactive. \"\n        }\n      ]\n    },\n    \"Test\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The questions for a Qualification test associated with this Qualification type that a user can take to obtain a Qualification of this type. This parameter must be specified if AnswerKey is present. A Qualification\
  \ type cannot have both a specified Test parameter and an AutoGranted value of true. \"\n        }\n      ]\n    },\n    \"TestDurationInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \" The amount of time, in seconds, given to a Worker to complete the Qualification test, beginning from the time the Worker requests the Qualification. \"\n        }\n      ]\n    },\n    \"AnswerKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The answers to the Qualification test specified in the Test parameter.\"\n        }\n      ]\n    },\n    \"RetryDelayInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \" The amount of time, in seconds, Workers must wait after taking the Qualification test before they can take\
  \ it again. Workers can take a Qualification test multiple times if they were not granted the Qualification from a previous attempt, or if the test offers a gradient score and they want a better score. If not specified, retries are disabled and Workers can request a Qualification only once. \"\n        }\n      ]\n    },\n    \"IsRequestable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \" Specifies whether the Qualification type is one that a user can request through the Amazon Mechanical Turk web site, such as by taking a Qualification test. This value is False for Qualifications assigned automatically by the system. Valid values are True | False. \"\n        }\n      ]\n    },\n    \"AutoGranted\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Specifies that requests for the Qualification type are\
  \ granted immediately, without prompting the Worker with a Qualification test. Valid values are True | False.\"\n        }\n      ]\n    },\n    \"AutoGrantedValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \" The Qualification integer value to use for automatically granted Qualifications, if AutoGranted is true. This is 1 by default. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-qualification-type-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: QualificationType
---
