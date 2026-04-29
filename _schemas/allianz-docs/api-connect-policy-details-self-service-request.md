---
description: Request body for creating a self-service policy completion session
layout: schema
name: PolicyDetailsSelfServiceRequest
properties_list:
- description: Unique identifier of the price estimate to complete
  name: estimate_id
  type: string
- description: URL to redirect customer back to after completing the policy
  name: redirect_url
  type: string
provider_name: Allianz
provider_slug: allianz-docs
schema_file: json-schema/api-connect-policy-details-self-service-request-schema.json
slug: api-connect-policy-details-self-service-request
source_filename: api-connect-policy-details-self-service-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-policy-details-self-service-request-schema.json\",\n  \"title\": \"PolicyDetailsSelfServiceRequest\",\n  \"description\": \"Request body for creating a self-service policy completion session\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"estimate_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the price estimate to complete\",\n      \"example\": \"est-500789\"\n    },\n    \"redirect_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to redirect customer back to after completing the policy\",\n      \"example\": \"https://portal.example.com/insurance/complete\"\n    }\n  },\n  \"required\": [\n    \"estimate_id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-policy-details-self-service-request-schema.json
tags:
- Financial Services
- Insurance
- Asset Management
title: PolicyDetailsSelfServiceRequest
---
