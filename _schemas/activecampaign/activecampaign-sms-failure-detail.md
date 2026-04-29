---
description: FailureDetail schema from ActiveCampaign API
layout: schema
name: FailureDetail
properties_list:
- description: ''
  name: errorCode
  type: string
- description: ''
  name: errorSource
  type: string
- description: ''
  name: count
  type: integer
provider_name: ActiveCampaign
provider_slug: activecampaign
schema_file: json-schema/activecampaign-sms-failure-detail-schema.json
slug: activecampaign-sms-failure-detail
source_filename: activecampaign-sms-failure-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/json-schema/activecampaign-sms-failure-detail-schema.json\",\n  \"title\": \"FailureDetail\",\n  \"description\": \"FailureDetail schema from ActiveCampaign API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorCode\": {\n      \"type\": \"string\"\n    },\n    \"errorSource\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ac\",\n        \"twilio\"\n      ]\n    },\n    \"count\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/json-schema/activecampaign-sms-failure-detail-schema.json
tags:
- Marketing Automation
- Email Marketing
- CRM
- Sales Automation
- Customer Experience
title: FailureDetail
---
