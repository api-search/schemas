---
description: SendBonusRequest schema from Amazon Mechanical Turk API
layout: schema
name: SendBonusRequest
properties_list:
- description: ''
  name: WorkerId
  type: object
- description: ''
  name: BonusAmount
  type: object
- description: ''
  name: AssignmentId
  type: object
- description: ''
  name: Reason
  type: object
- description: ''
  name: UniqueRequestToken
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-send-bonus-request-schema.json
slug: amazon-mechanical-turk-send-bonus-request
source_filename: amazon-mechanical-turk-send-bonus-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-send-bonus-request-schema.json\",\n  \"title\": \"SendBonusRequest\",\n  \"description\": \"SendBonusRequest schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"WorkerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomerId\"\n        },\n        {\n          \"description\": \"The ID of the Worker being paid the bonus.\"\n        }\n      ]\n    },\n    \"BonusAmount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CurrencyAmount\"\n        },\n        {\n          \"description\": \" The Bonus amount is a US Dollar amount specified using a string (for example, \\\"5\\\" represents $5.00 USD and \\\"101.42\\\" represents $101.42 USD). Do not include currency symbols\
  \ or currency codes. \"\n        }\n      ]\n    },\n    \"AssignmentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \"The ID of the assignment for which this bonus is paid.\"\n        }\n      ]\n    },\n    \"Reason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A message that explains the reason for the bonus payment. The Worker receiving the bonus can see this message.\"\n        }\n      ]\n    },\n    \"UniqueRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdempotencyToken\"\n        },\n        {\n          \"description\": \"A unique identifier for this request, which allows you to retry the call on error without granting multiple bonuses. This is useful in cases such as network timeouts where it is unclear whether or not the call succeeded on the\
  \ server. If the bonus already exists in the system from a previous call using the same UniqueRequestToken, subsequent calls will return an error with a message containing the request ID.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"WorkerId\",\n    \"BonusAmount\",\n    \"AssignmentId\",\n    \"Reason\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-send-bonus-request-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: SendBonusRequest
---
