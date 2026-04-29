---
description: An object that describes workflow billing details.
layout: schema
name: BillingDetails
properties_list:
- description: ''
  name: billedMemoryUsedInMB
  type: object
- description: ''
  name: billedDurationInMilliseconds
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-billing-details-schema.json
slug: amazon-step-functions-billing-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-billing-details-schema.json\",\n  \"title\": \"BillingDetails\",\n  \"description\": \"An object that describes workflow billing details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"billedMemoryUsedInMB\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BilledMemoryUsed\"\n        },\n        {\n          \"description\": \"Billed memory consumption of your workflow, in MB.\"\n        }\n      ]\n    },\n    \"billedDurationInMilliseconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BilledDuration\"\n        },\n        {\n          \"description\": \"Billed duration of your workflow, in milliseconds.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-billing-details-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: BillingDetails
---
