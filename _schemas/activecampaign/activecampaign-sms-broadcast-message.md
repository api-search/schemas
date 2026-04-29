---
description: BroadcastMessage schema from ActiveCampaign API
layout: schema
name: BroadcastMessage
properties_list:
- description: Unique identifier for the broadcast
  name: id
  type: integer
- description: Name of the broadcast
  name: name
  type: string
- description: ID used to get sender name
  name: address_id
  type: integer
- description: SMS message content
  name: body
  type: string
- description: Media URLs for MMS messages
  name: media_urls
  type: array
- description: URL for message preview
  name: preview_url
  type: string
- description: Whether link shortening is enabled
  name: shorten_track_links_enabled
  type: boolean
- description: Current status of the broadcast
  name: status
  type: string
- description: Date when broadcast was sent
  name: sent_date
  type: string
- description: Scheduled send date (UTC)
  name: scheduled_date
  type: string
- description: custom run id generated from segmentMatchSome endpoint
  name: custom_run_id
  type: string
- description: custom segment id generated from segmentsV2 endpoint and passing in a valid audience
  name: custom_segment_id
  type: string
- description: User ID who scheduled the broadcast
  name: scheduled_by
  type: integer
- description: Number of recipients
  name: sent_to_count
  type: integer
- description: Creation timestamp
  name: created_at
  type: string
- description: User ID who created the broadcast
  name: created_by
  type: integer
- description: Last update timestamp
  name: updated_at
  type: string
- description: User ID who last updated
  name: updated_by
  type: integer
- description: Deletion timestamp (for soft deletes)
  name: deleted_at
  type: string
- description: Sift approval status
  name: sift_approved
  type: integer
- description: ARC approval status
  name: arc_approved
  type: integer
- description: Whether quiet hours are enabled
  name: quiet_hours_enabled
  type: integer
- description: Associated list IDs
  name: list_ids
  type: array
- description: Segment ID (can be UUID or integer string)
  name: segment_id
  type: string
- description: Associated label IDs
  name: label_ids
  type: array
provider_name: ActiveCampaign
provider_slug: activecampaign
schema_file: json-schema/activecampaign-sms-broadcast-message-schema.json
slug: activecampaign-sms-broadcast-message
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/json-schema/activecampaign-sms-broadcast-message-schema.json\",\n  \"title\": \"BroadcastMessage\",\n  \"description\": \"BroadcastMessage schema from ActiveCampaign API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the broadcast\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the broadcast\"\n    },\n    \"address_id\": {\n      \"type\": \"integer\",\n      \"nullable\": true,\n      \"description\": \"ID used to get sender name\"\n    },\n    \"body\": {\n      \"type\": \"string\",\n      \"description\": \"SMS message content\"\n    },\n    \"media_urls\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uri\"\n      },\n\
  \      \"description\": \"Media URLs for MMS messages\"\n    },\n    \"preview_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL for message preview\"\n    },\n    \"shorten_track_links_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether link shortening is enabled\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"draft\",\n        \"scheduled\",\n        \"sent\",\n        \"pending_review\",\n        \"sending\"\n      ],\n      \"description\": \"Current status of the broadcast\"\n    },\n    \"sent_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"description\": \"Date when broadcast was sent\"\n    },\n    \"scheduled_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"description\": \"Scheduled send date (UTC)\"\n    },\n    \"custom_run_id\": {\n      \"type\"\
  : \"string\",\n      \"format\": \"uuid\",\n      \"nullable\": true,\n      \"description\": \"custom run id generated from segmentMatchSome endpoint\"\n    },\n    \"custom_segment_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"nullable\": true,\n      \"description\": \"custom segment id generated from segmentsV2 endpoint and passing in a valid audience\"\n    },\n    \"scheduled_by\": {\n      \"type\": \"integer\",\n      \"nullable\": true,\n      \"description\": \"User ID who scheduled the broadcast\"\n    },\n    \"sent_to_count\": {\n      \"type\": \"integer\",\n      \"nullable\": true,\n      \"description\": \"Number of recipients\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Creation timestamp\"\n    },\n    \"created_by\": {\n      \"type\": \"integer\",\n      \"description\": \"User ID who created the broadcast\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"Last update timestamp\"\n    },\n    \"updated_by\": {\n      \"type\": \"integer\",\n      \"description\": \"User ID who last updated\"\n    },\n    \"deleted_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"description\": \"Deletion timestamp (for soft deletes)\"\n    },\n    \"sift_approved\": {\n      \"type\": \"integer\",\n      \"description\": \"Sift approval status\"\n    },\n    \"arc_approved\": {\n      \"type\": \"integer\",\n      \"description\": \"ARC approval status\"\n    },\n    \"quiet_hours_enabled\": {\n      \"type\": \"integer\",\n      \"nullable\": true,\n      \"description\": \"Whether quiet hours are enabled\"\n    },\n    \"list_ids\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      },\n      \"description\": \"Associated list IDs\"\n    },\n    \"segment_id\": {\n      \"type\": \"string\",\n    \
  \  \"nullable\": true,\n      \"description\": \"Segment ID (can be UUID or integer string)\"\n    },\n    \"label_ids\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      },\n      \"nullable\": true,\n      \"description\": \"Associated label IDs\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/json-schema/activecampaign-sms-broadcast-message-schema.json
tags:
- Marketing Automation
- Email Marketing
- CRM
- Sales Automation
- Customer Experience
title: BroadcastMessage
---
