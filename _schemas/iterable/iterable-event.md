---
description: A tracked event in Iterable representing a user action or system activity. Events are used to trigger campaigns, segment users, and track engagement metrics across the marketing automation platform.
layout: schema
name: Iterable Event
properties_list:
- description: Email address of the user associated with the event
  name: email
  type: string
- description: Alternative user identifier for the event
  name: userId
  type: string
- description: Name of the event, used to identify the event type in campaign triggers and segmentation
  name: eventName
  type: string
- description: Unix timestamp in milliseconds of when the event occurred
  name: createdAt
  type: integer
- description: Custom data fields containing event-specific details for personalization and filtering
  name: dataFields
  type: object
- description: Campaign ID to attribute this event to
  name: campaignId
  type: integer
- description: Template ID to attribute this event to
  name: templateId
  type: integer
provider_name: Iterable
provider_slug: iterable
schema_file: json-schema/iterable-event-schema.json
slug: iterable-event
source_filename: iterable-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.api-evangelist.com/schemas/iterable/event.json\",\n  \"title\": \"Iterable Event\",\n  \"description\": \"A tracked event in Iterable representing a user action or system activity. Events are used to trigger campaigns, segment users, and track engagement metrics across the marketing automation platform.\",\n  \"type\": \"object\",\n  \"required\": [\"eventName\"],\n  \"properties\": {\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address of the user associated with the event\"\n    },\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"Alternative user identifier for the event\"\n    },\n    \"eventName\": {\n      \"type\": \"string\",\n      \"minLength\": 1,\n      \"description\": \"Name of the event, used to identify the event type in campaign triggers and segmentation\"\n    },\n    \"createdAt\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp in milliseconds of when the event occurred\"\n    },\n    \"dataFields\": {\n      \"type\": \"object\",\n      \"description\": \"Custom data fields containing event-specific details for personalization and filtering\",\n      \"additionalProperties\": true\n    },\n    \"campaignId\": {\n      \"type\": \"integer\",\n      \"description\": \"Campaign ID to attribute this event to\"\n    },\n    \"templateId\": {\n      \"type\": \"integer\",\n      \"description\": \"Template ID to attribute this event to\"\n    }\n  },\n  \"anyOf\": [\n    {\"required\": [\"email\"]},\n    {\"required\": [\"userId\"]}\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/iterable/refs/heads/main/json-schema/iterable-event-schema.json
tags:
- Cross-Channel Messaging
- Customer Engagement
- Email
- Marketing Automation
- Push Notifications
- SMS
title: Iterable Event
---
