---
description: A marketing campaign in Iterable that delivers messages to targeted audiences across email, push, SMS, and in-app channels. Campaigns can be blast sends to lists, triggered by events or API calls, or proof/test sends.
layout: schema
name: Iterable Campaign
properties_list:
- description: Unique campaign identifier
  name: id
  type: integer
- description: Human-readable campaign name
  name: name
  type: string
- description: The type of campaign
  name: type
  type: string
- description: ID of the message template used by this campaign
  name: templateId
  type: integer
- description: ISO 8601 timestamp of when the campaign was created
  name: createdAt
  type: string
- description: ISO 8601 timestamp of when the campaign was last modified
  name: updatedAt
  type: string
- description: ISO 8601 timestamp of the scheduled start time
  name: startAt
  type: string
- description: ISO 8601 timestamp of when the campaign finished sending
  name: endedAt
  type: string
- description: The messaging channel used by this campaign
  name: messageMedium
  type: string
- description: Current state of the campaign lifecycle
  name: campaignState
  type: string
- description: IDs of lists targeted by this campaign
  name: listIds
  type: array
- description: IDs of suppression lists to exclude from targeting
  name: suppressionListIds
  type: array
- description: Labels applied to the campaign for organization
  name: labels
  type: array
- description: ID of the workflow this campaign belongs to, if applicable
  name: workflowId
  type: integer
- description: Custom data fields for campaign-level personalization
  name: dataFields
  type: object
provider_name: Iterable
provider_slug: iterable
schema_file: json-schema/iterable-campaign-schema.json
slug: iterable-campaign
source_filename: iterable-campaign-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.api-evangelist.com/schemas/iterable/campaign.json\",\n  \"title\": \"Iterable Campaign\",\n  \"description\": \"A marketing campaign in Iterable that delivers messages to targeted audiences across email, push, SMS, and in-app channels. Campaigns can be blast sends to lists, triggered by events or API calls, or proof/test sends.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique campaign identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"minLength\": 1,\n      \"description\": \"Human-readable campaign name\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"Blast\", \"Triggered\", \"Proof\"],\n      \"description\": \"The type of campaign\"\n    },\n    \"templateId\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"ID of the message template used by this campaign\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of when the campaign was created\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of when the campaign was last modified\"\n    },\n    \"startAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of the scheduled start time\"\n    },\n    \"endedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of when the campaign finished sending\"\n    },\n    \"messageMedium\": {\n      \"type\": \"string\",\n      \"enum\": [\"Email\", \"Push\", \"SMS\", \"InApp\", \"WebPush\"],\n      \"description\": \"The messaging channel used by this campaign\"\n    },\n    \"campaignState\": {\n      \"\
  type\": \"string\",\n      \"enum\": [\"Draft\", \"Scheduled\", \"Running\", \"Finished\", \"Cancelled\"],\n      \"description\": \"Current state of the campaign lifecycle\"\n    },\n    \"listIds\": {\n      \"type\": \"array\",\n      \"description\": \"IDs of lists targeted by this campaign\",\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"suppressionListIds\": {\n      \"type\": \"array\",\n      \"description\": \"IDs of suppression lists to exclude from targeting\",\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"description\": \"Labels applied to the campaign for organization\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"workflowId\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the workflow this campaign belongs to, if applicable\"\n    },\n    \"dataFields\": {\n      \"type\": \"object\",\n      \"description\": \"Custom data\
  \ fields for campaign-level personalization\",\n      \"additionalProperties\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/iterable/refs/heads/main/json-schema/iterable-campaign-schema.json
tags:
- Cross-Channel Messaging
- Customer Engagement
- Email
- Marketing Automation
- Push Notifications
- SMS
title: Iterable Campaign
---
