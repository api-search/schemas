---
description: AcceptQualificationRequestRequest schema from Amazon Mechanical Turk API
layout: schema
name: AcceptQualificationRequestRequest
properties_list:
- description: ''
  name: QualificationRequestId
  type: object
- description: ''
  name: IntegerValue
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-accept-qualification-request-request-schema.json
slug: amazon-mechanical-turk-accept-qualification-request-request
source_filename: amazon-mechanical-turk-accept-qualification-request-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-accept-qualification-request-request-schema.json\",\n  \"title\": \"AcceptQualificationRequestRequest\",\n  \"description\": \"AcceptQualificationRequestRequest schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"QualificationRequestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The ID of the Qualification request, as returned by the <code>GetQualificationRequests</code> operation.\"\n        }\n      ]\n    },\n    \"IntegerValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \" The value of the Qualification. You can omit this value if you\
  \ are using the presence or absence of the Qualification as the basis for a HIT requirement. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"QualificationRequestId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-accept-qualification-request-request-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: AcceptQualificationRequestRequest
---
