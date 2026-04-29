---
description: SOAP envelope containing the service name and recipient DOM element for subscribe/unsubscribe operations.
layout: schema
name: SubscriptionRequest
properties_list:
- description: Internal name of the information service.
  name: serviceName
  type: string
- description: Recipient DOM element identifying the subscriber.
  name: recipient
  type: object
- description: Whether to create the recipient if not found (subscribe only).
  name: create
  type: boolean
provider_name: Adobe Campaign
provider_slug: adobe-campaign
schema_file: json-schema/adobe-campaign-classic-subscription-request-schema.json
slug: adobe-campaign-classic-subscription-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-classic-subscription-request-schema.json\",\n  \"title\": \"SubscriptionRequest\",\n  \"description\": \"SOAP envelope containing the service name and recipient DOM element for subscribe/unsubscribe operations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serviceName\": {\n      \"type\": \"string\",\n      \"description\": \"Internal name of the information service.\",\n      \"example\": \"Example Campaign\"\n    },\n    \"recipient\": {\n      \"type\": \"object\",\n      \"description\": \"Recipient DOM element identifying the subscriber.\",\n      \"properties\": {\n        \"email\": {\n          \"type\": \"string\",\n          \"description\": \"Email address of the recipient.\"\n        },\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\"\
  : \"Internal ID of the recipient.\"\n        }\n      }\n    },\n    \"create\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to create the recipient if not found (subscribe only).\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-classic-subscription-request-schema.json
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
title: SubscriptionRequest
---
