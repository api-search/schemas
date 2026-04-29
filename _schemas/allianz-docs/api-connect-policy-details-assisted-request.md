---
description: Request body for staff-assisted policy details completion
layout: schema
name: PolicyDetailsAssistedRequest
properties_list:
- description: Unique identifier of the price estimate to convert
  name: estimate_id
  type: string
- description: Unique identifier of the customer
  name: customer_id
  type: string
- description: Preferred payment frequency for the policy
  name: payment_frequency
  type: string
provider_name: Allianz
provider_slug: allianz-docs
schema_file: json-schema/api-connect-policy-details-assisted-request-schema.json
slug: api-connect-policy-details-assisted-request
source_filename: api-connect-policy-details-assisted-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-policy-details-assisted-request-schema.json\",\n  \"title\": \"PolicyDetailsAssistedRequest\",\n  \"description\": \"Request body for staff-assisted policy details completion\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"estimate_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the price estimate to convert\",\n      \"example\": \"est-500123\"\n    },\n    \"customer_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the customer\",\n      \"example\": \"500123\"\n    },\n    \"payment_frequency\": {\n      \"type\": \"string\",\n      \"description\": \"Preferred payment frequency for the policy\",\n      \"enum\": [\n        \"annual\",\n        \"monthly\"\n      ],\n      \"example\": \"monthly\"\n    }\n  },\n\
  \  \"required\": [\n    \"estimate_id\",\n    \"customer_id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-policy-details-assisted-request-schema.json
tags:
- Financial Services
- Insurance
- Asset Management
title: PolicyDetailsAssistedRequest
---
