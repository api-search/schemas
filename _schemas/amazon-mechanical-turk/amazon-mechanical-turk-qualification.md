---
description: The Qualification data structure represents a Qualification assigned to a user, including the Qualification type and the value (score).
layout: schema
name: Qualification
properties_list:
- description: ''
  name: QualificationTypeId
  type: object
- description: ''
  name: WorkerId
  type: object
- description: ''
  name: GrantTime
  type: object
- description: ''
  name: IntegerValue
  type: object
- description: ''
  name: LocaleValue
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-qualification-schema.json
slug: amazon-mechanical-turk-qualification
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-qualification-schema.json\",\n  \"title\": \"Qualification\",\n  \"description\": \"The Qualification data structure represents a Qualification assigned to a user, including the Qualification type and the value (score).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"QualificationTypeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \" The ID of the Qualification type for the Qualification.\"\n        }\n      ]\n    },\n    \"WorkerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomerId\"\n        },\n        {\n          \"description\": \" The ID of the Worker who possesses the Qualification. \"\n        }\n      ]\n    },\n    \"\
  GrantTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" The date and time the Qualification was granted to the Worker. If the Worker's Qualification was revoked, and then re-granted based on a new Qualification request, GrantTime is the date and time of the last call to the AcceptQualificationRequest operation.\"\n        }\n      ]\n    },\n    \"IntegerValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \" The value (score) of the Qualification, if the Qualification has an integer value.\"\n        }\n      ]\n    },\n    \"LocaleValue\": {\n      \"$ref\": \"#/components/schemas/Locale\"\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QualificationStatus\"\n        },\n        {\n          \"description\": \" The status of the Qualification.\
  \ Valid values are Granted | Revoked.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-qualification-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: Qualification
---
