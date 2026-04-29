---
description: PrivacyRequestResponse from Adobe Campaign API
layout: schema
name: PrivacyRequestResponse
properties_list:
- description: The PKEY of the created privacy request.
  name: PKey
  type: string
- description: Current status of the privacy request.
  name: status
  type: string
provider_name: Adobe Campaign
provider_slug: adobe-campaign
schema_file: json-schema/adobe-campaign-standard-privacy-request-response-schema.json
slug: adobe-campaign-standard-privacy-request-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-standard-privacy-request-response-schema.json\",\n  \"title\": \"PrivacyRequestResponse\",\n  \"description\": \"PrivacyRequestResponse from Adobe Campaign API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PKey\": {\n      \"type\": \"string\",\n      \"description\": \"The PKEY of the created privacy request.\",\n      \"example\": \"example_value\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the privacy request.\",\n      \"example\": \"active\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-standard-privacy-request-response-schema.json
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
title: PrivacyRequestResponse
---
