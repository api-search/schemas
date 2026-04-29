---
description: Schema for a Constant Contact V3 email campaign and campaign activity.
layout: schema
name: Constant Contact Email Campaign
properties_list:
- description: ''
  name: campaign_id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: type_code
  type: integer
- description: ''
  name: current_status
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
- description: ''
  name: campaign_activities
  type: array
provider_name: Constant Contact
provider_slug: constant-contact
schema_file: json-schema/constant-contact-campaign-schema.json
slug: constant-contact-campaign
source_filename: constant-contact-campaign-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/json-schema/constant-contact-campaign-schema.json\",\n  \"title\": \"Constant Contact Email Campaign\",\n  \"description\": \"Schema for a Constant Contact V3 email campaign and campaign activity.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"campaign_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"maxLength\": 80\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"NEWSLETTER\", \"ANNOUNCEMENT\", \"PRODUCT_PROMOTION\", \"ABANDONED_CART\", \"WELCOME\", \"BIRTHDAY\", \"ANNIVERSARY\", \"RESEND\", \"EVENT\", \"CUSTOM_CODE\", \"A_B_TEST\"]\n    },\n    \"type_code\": { \"type\": \"integer\" },\n    \"current_status\": {\n      \"type\": \"string\",\n      \"enum\": [\"NONE\", \"DRAFT\", \"SCHEDULED\", \"EXECUTING\"\
  , \"DONE\", \"ERROR\", \"REMOVED\"]\n    },\n    \"created_at\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"updated_at\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"campaign_activities\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"campaign_activity_id\": { \"type\": \"string\", \"format\": \"uuid\" },\n          \"role\": {\n            \"type\": \"string\",\n            \"enum\": [\"primary_email\", \"resend\", \"permalink\", \"winner_resend\", \"ab_a\", \"ab_b\"]\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"name\"],\n  \"definitions\": {\n    \"EmailCampaignActivity\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"campaign_activity_id\": { \"type\": \"string\", \"format\": \"uuid\" },\n        \"campaign_id\": { \"type\": \"string\", \"format\": \"uuid\" },\n        \"role\": {\n          \"type\": \"string\",\n          \"enum\": [\"\
  primary_email\", \"resend\", \"permalink\", \"winner_resend\", \"ab_a\", \"ab_b\"]\n        },\n        \"current_status\": {\n          \"type\": \"string\",\n          \"enum\": [\"DRAFT\", \"SCHEDULED\", \"EXECUTING\", \"DONE\", \"ERROR\", \"REMOVED\"]\n        },\n        \"from_email\": { \"type\": \"string\", \"format\": \"email\" },\n        \"from_name\": { \"type\": \"string\", \"maxLength\": 100 },\n        \"reply_to_email\": { \"type\": \"string\", \"format\": \"email\" },\n        \"subject\": { \"type\": \"string\", \"maxLength\": 200 },\n        \"preheader\": { \"type\": \"string\", \"maxLength\": 250 },\n        \"html_content\": { \"type\": \"string\" },\n        \"physical_address_in_footer\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"address_line1\": { \"type\": \"string\" },\n            \"address_line2\": { \"type\": \"string\" },\n            \"city\": { \"type\": \"string\" },\n            \"state_code\": { \"type\": \"string\"\
  \ },\n            \"country_code\": { \"type\": \"string\" },\n            \"organization_name\": { \"type\": \"string\" },\n            \"postal_code\": { \"type\": \"string\" }\n          }\n        },\n        \"contact_list_ids\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\", \"format\": \"uuid\" }\n        },\n        \"segment_ids\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"integer\" }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/json-schema/constant-contact-campaign-schema.json
tags:
- Campaigns
- Contacts
- Email Marketing
- Events
- Reporting
- SMS
- Surveys
title: Constant Contact Email Campaign
---
