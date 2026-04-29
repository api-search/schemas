---
description: SubscriptionRequest from Adobe Campaign API
layout: schema
name: SubscriptionRequest
properties_list:
- description: ''
  name: service
  type: object
provider_name: Adobe Campaign
provider_slug: adobe-campaign
schema_file: json-schema/adobe-campaign-standard-subscription-request-schema.json
slug: adobe-campaign-standard-subscription-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-standard-subscription-request-schema.json\",\n  \"title\": \"SubscriptionRequest\",\n  \"description\": \"SubscriptionRequest from Adobe Campaign API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"service\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"PKey\": {\n          \"type\": \"string\",\n          \"description\": \"The PKEY of the service to subscribe to.\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"service\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-standard-subscription-request-schema.json
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
title: SubscriptionRequest
---
