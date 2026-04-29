---
description: Request body for creating a design autofill job
layout: schema
name: CreateAutofillJobRequest
properties_list:
- description: The brand template ID to autofill
  name: brand_template_id
  type: string
- description: Title for the generated design (1-255 characters). Defaults to the brand template title.
  name: title
  type: string
- description: Data fields to populate, keyed by field name from the brand template dataset
  name: data
  type: object
provider_name: Canva
provider_slug: canva
schema_file: json-schema/canva-connect-create-autofill-job-request-schema.json
slug: canva-connect-create-autofill-job-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateAutofillJobRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a design autofill job\",\n  \"properties\": {\n    \"brand_template_id\": {\n      \"type\": \"string\",\n      \"description\": \"The brand template ID to autofill\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title for the generated design (1-255 characters). Defaults to the brand template title.\"\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"Data fields to populate, keyed by field name from the brand template dataset\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-create-autofill-job-request-schema.json
tags:
- Apps
- Automation
- Brand Management
- Collaboration
- Design
- Graphics
- Marketing
- Print
- Templates
- Visual Content
title: CreateAutofillJobRequest
---
