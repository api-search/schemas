---
description: HIT Review Policy data structures represent HIT review policies, which you specify when you create a HIT.
layout: schema
name: ReviewPolicy
properties_list:
- description: ''
  name: PolicyName
  type: object
- description: ''
  name: Parameters
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-review-policy-schema.json
slug: amazon-mechanical-turk-review-policy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-review-policy-schema.json\",\n  \"title\": \"ReviewPolicy\",\n  \"description\": \" HIT Review Policy data structures represent HIT review policies, which you specify when you create a HIT. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PolicyName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" Name of a Review Policy: SimplePlurality/2011-09-01 or ScoreMyKnownAnswers/2011-09-01 \"\n        }\n      ]\n    },\n    \"Parameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyParameterList\"\n        },\n        {\n          \"description\": \"Name of the parameter from the Review policy.\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"PolicyName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-review-policy-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: ReviewPolicy
---
