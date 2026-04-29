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
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-billingdetails-schema.json
slug: step-functions-billingdetails
source_filename: step-functions-billingdetails-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BillingDetails\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"billedMemoryUsedInMB\": {},\n    \"billedDurationInMilliseconds\": {}\n  },\n  \"description\": \"An object that describes workflow billing details.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-billingdetails-schema.json
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: BillingDetails
---
