---
description: CollectionResponseMeeting schema from HubSpot Engagement Meetings API
layout: schema
name: CollectionResponseMeeting
properties_list:
- description: ''
  name: results
  type: array
- description: ''
  name: paging
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/engagement-meetings-api-collection-response-meeting-schema.json
slug: engagement-meetings-api-collection-response-meeting
source_filename: engagement-meetings-api-collection-response-meeting-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-meetings-api-collection-response-meeting-schema.json\",\n  \"title\": \"CollectionResponseMeeting\",\n  \"description\": \"CollectionResponseMeeting schema from HubSpot Engagement Meetings API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A HubSpot meeting engagement record.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier for the meeting.\",\n            \"example\": \"500123\"\n          },\n          \"properties\": {\n            \"type\": \"object\",\n            \"description\": \"The meeting's properties as key-value pairs.\",\n            \"additionalProperties\": {\n      \
  \        \"type\": \"string\"\n            },\n            \"example\": {\n              \"key\": \"value\"\n            }\n          },\n          \"createdAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"updatedAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"archived\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"associations\": {\n            \"type\": \"object\",\n            \"additionalProperties\": {\n              \"$ref\": \"#/components/schemas/CollectionResponseAssociation\"\n            },\n            \"example\": {\n              \"key\": \"value\"\n            }\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"id\": \"500123\",\n          \"properties\": {\n          \
  \  \"key\": \"value\"\n          },\n          \"createdAt\": \"2025-03-15T14:30:00Z\",\n          \"updatedAt\": \"2025-03-15T14:30:00Z\",\n          \"archived\": true,\n          \"associations\": {\n            \"key\": \"value\"\n          }\n        }\n      ]\n    },\n    \"paging\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"after\": {\n              \"type\": \"string\"\n            }\n          },\n          \"example\": {\n            \"after\": \"example-value\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-meetings-api-collection-response-meeting-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: CollectionResponseMeeting
---
