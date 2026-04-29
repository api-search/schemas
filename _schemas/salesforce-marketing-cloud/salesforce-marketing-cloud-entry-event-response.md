---
description: Response returned after firing a journey entry event
layout: schema
name: EntryEventResponse
properties_list:
- description: Unique identifier for the event request
  name: requestId
  type: string
- description: Unique instance identifier for this event firing
  name: eventInstanceId
  type: string
provider_name: Salesforce Marketing Cloud
provider_slug: salesforce-marketing-cloud
schema_file: json-schema/salesforce-marketing-cloud-entry-event-response-schema.json
slug: salesforce-marketing-cloud-entry-event-response
source_filename: salesforce-marketing-cloud-entry-event-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EntryEventResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response returned after firing a journey entry event\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the event request\"\n    },\n    \"eventInstanceId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique instance identifier for this event firing\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/json-schema/salesforce-marketing-cloud-entry-event-response-schema.json
tags:
- Automation
- Customer Journey
- Digital Marketing
- Email
- Marketing
- Personalization
title: EntryEventResponse
---
