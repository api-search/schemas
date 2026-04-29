---
description: FailureDetailsResponse schema from ActiveCampaign API
layout: schema
name: FailureDetailsResponse
properties_list:
- description: ''
  name: failures
  type: array
provider_name: ActiveCampaign
provider_slug: activecampaign
schema_file: json-schema/activecampaign-sms-failure-details-response-schema.json
slug: activecampaign-sms-failure-details-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/json-schema/activecampaign-sms-failure-details-response-schema.json\",\n  \"title\": \"FailureDetailsResponse\",\n  \"description\": \"FailureDetailsResponse schema from ActiveCampaign API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"failures\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/FailureDetail\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/json-schema/activecampaign-sms-failure-details-response-schema.json
tags:
- Marketing Automation
- Email Marketing
- CRM
- Sales Automation
- Customer Experience
title: FailureDetailsResponse
---
