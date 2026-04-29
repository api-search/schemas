---
description: SOAP envelope containing a real-time event for transactional message processing. The rtEvent element includes mandatory attributes for event type and recipient contact, plus a ctx child element for message personalization data.
layout: schema
name: PushEventRequest
properties_list:
- description: ''
  name: rtEvent
  type: object
provider_name: Adobe Campaign
provider_slug: adobe-campaign
schema_file: json-schema/adobe-campaign-classic-push-event-request-schema.json
slug: adobe-campaign-classic-push-event-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-classic-push-event-request-schema.json\",\n  \"title\": \"PushEventRequest\",\n  \"description\": \"SOAP envelope containing a real-time event for transactional message processing. The rtEvent element includes mandatory attributes for event type and recipient contact, plus a ctx child element for message personalization data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"rtEvent\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Event type name matching the Message Center event configuration.\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"Recipient email address.\"\n        },\n        \"origin\": {\n  \
  \        \"type\": \"string\",\n          \"description\": \"Origin identifier for tracking the event source.\"\n        },\n        \"wishedChannel\": {\n          \"type\": \"integer\",\n          \"description\": \"Preferred delivery channel. 0 = email, 1 = mobile (SMS), 2 = phone, 3 = push notification.\"\n        },\n        \"externalId\": {\n          \"type\": \"string\",\n          \"description\": \"External identifier for deduplication.\"\n        },\n        \"mobilePhone\": {\n          \"type\": \"string\",\n          \"description\": \"Recipient mobile phone number (for SMS channel).\"\n        },\n        \"scheduled\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Optional scheduled processing time.\"\n        },\n        \"ctx\": {\n          \"type\": \"object\",\n          \"description\": \"Context data XML element containing personalization variables for the transactional message template.\",\n          \"additionalProperties\"\
  : true\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-classic-push-event-request-schema.json
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
title: PushEventRequest
---
