---
description: An object representing a Bonus payment paid to a Worker.
layout: schema
name: BonusPayment
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
  name: GrantTime
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-bonus-payment-schema.json
slug: amazon-mechanical-turk-bonus-payment
source_filename: amazon-mechanical-turk-bonus-payment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-bonus-payment-schema.json\",\n  \"title\": \"BonusPayment\",\n  \"description\": \"An object representing a Bonus payment paid to a Worker.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"WorkerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomerId\"\n        },\n        {\n          \"description\": \"The ID of the Worker to whom the bonus was paid.\"\n        }\n      ]\n    },\n    \"BonusAmount\": {\n      \"$ref\": \"#/components/schemas/CurrencyAmount\"\n    },\n    \"AssignmentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityId\"\n        },\n        {\n          \"description\": \"The ID of the assignment associated with this bonus payment.\"\n        }\n      ]\n    },\n    \"Reason\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Reason text given when the bonus was granted, if any.\"\n        }\n      ]\n    },\n    \"GrantTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time of when the bonus was granted.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-bonus-payment-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: BonusPayment
---
