---
description: DisassociateQualificationFromWorkerRequest schema from Amazon Mechanical Turk API
layout: schema
name: DisassociateQualificationFromWorkerRequest
properties_list:
- description: ''
  name: WorkerId
  type: object
- description: ''
  name: QualificationTypeId
  type: object
- description: ''
  name: Reason
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-disassociate-qualification-from-worker-request-schema.json
slug: amazon-mechanical-turk-disassociate-qualification-from-worker-request
source_filename: amazon-mechanical-turk-disassociate-qualification-from-worker-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-disassociate-qualification-from-worker-request-schema.json\",\n  \"title\": \"DisassociateQualificationFromWorkerRequest\",\n  \"description\": \"DisassociateQualificationFromWorkerRequest schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"WorkerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomerId\"\n        },\n        {\n          \"description\": \"The ID of the Worker who possesses the Qualification to be revoked.\"\n        }\n      ]\n    },\n    \"QualificationTypeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \"The ID of the Qualification type of the Qualification to be revoked.\"\n  \
  \      }\n      ]\n    },\n    \"Reason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A text message that explains why the Qualification was revoked. The user who had the Qualification sees this message.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"WorkerId\",\n    \"QualificationTypeId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-disassociate-qualification-from-worker-request-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: DisassociateQualificationFromWorkerRequest
---
