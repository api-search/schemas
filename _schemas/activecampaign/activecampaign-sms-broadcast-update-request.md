---
description: BroadcastUpdateRequest schema from ActiveCampaign API
layout: schema
name: BroadcastUpdateRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: address_id
  type: integer
- description: ''
  name: body
  type: string
- description: ''
  name: media_urls
  type: array
- description: ''
  name: preview_url
  type: string
- description: ''
  name: shorten_track_links_enabled
  type: boolean
- description: Status of the broadcast. pending_review starts kicks off the broadcast to be sent
  name: status
  type: string
- description: ''
  name: scheduled_date
  type: string
- description: ''
  name: sent_to_count
  type: integer
- description: ''
  name: list_ids
  type: array
- description: ''
  name: segment_id
  type: string
- description: custom run id generated from segmentMatchSome endpoint and passing a valid segment id
  name: custom_run_id
  type: string
- description: custom segment id generated from segmentsV2 endpoint and passing in a valid audience
  name: custom_segment_id
  type: string
- description: ''
  name: label_ids
  type: array
provider_name: ActiveCampaign
provider_slug: activecampaign
schema_file: json-schema/activecampaign-sms-broadcast-update-request-schema.json
slug: activecampaign-sms-broadcast-update-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/json-schema/activecampaign-sms-broadcast-update-request-schema.json\",\n  \"title\": \"BroadcastUpdateRequest\",\n  \"description\": \"BroadcastUpdateRequest schema from ActiveCampaign API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"address_id\": {\n      \"type\": \"integer\",\n      \"nullable\": true\n    },\n    \"body\": {\n      \"type\": \"string\"\n    },\n    \"media_urls\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uri\"\n      }\n    },\n    \"preview_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\"\n    },\n    \"shorten_track_links_enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of\
  \ the broadcast. pending_review starts kicks off the broadcast to be sent\",\n      \"enum\": [\n        \"draft\",\n        \"pending_review\"\n      ]\n    },\n    \"scheduled_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"sent_to_count\": {\n      \"type\": \"integer\"\n    },\n    \"list_ids\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"segment_id\": {\n      \"type\": \"string\"\n    },\n    \"custom_run_id\": {\n      \"type\": \"string\",\n      \"description\": \"custom run id generated from segmentMatchSome endpoint and passing a valid segment id\",\n      \"format\": \"uuid\",\n      \"nullable\": true\n    },\n    \"custom_segment_id\": {\n      \"type\": \"string\",\n      \"description\": \"custom segment id generated from segmentsV2 endpoint and passing in a valid audience\",\n      \"format\": \"uuid\",\n      \"nullable\": true\n    },\n    \"label_ids\": {\n      \"type\"\
  : \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/json-schema/activecampaign-sms-broadcast-update-request-schema.json
tags:
- Marketing Automation
- Email Marketing
- CRM
- Sales Automation
- Customer Experience
title: BroadcastUpdateRequest
---
