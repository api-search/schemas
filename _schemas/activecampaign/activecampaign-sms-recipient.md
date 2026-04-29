---
description: Recipient schema from ActiveCampaign API
layout: schema
name: Recipient
properties_list:
- description: Contact ID
  name: id
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: phoneNumber
  type: string
- description: Timestamp in CST
  name: sentDate
  type: string
- description: ''
  name: clicks
  type: integer
- description: ''
  name: deliverability
  type: string
- description: ''
  name: replies
  type: array
- description: ''
  name: optOut
  type: string
- description: ''
  name: details
  type: object
provider_name: ActiveCampaign
provider_slug: activecampaign
schema_file: json-schema/activecampaign-sms-recipient-schema.json
slug: activecampaign-sms-recipient
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/json-schema/activecampaign-sms-recipient-schema.json\",\n  \"title\": \"Recipient\",\n  \"description\": \"Recipient schema from ActiveCampaign API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Contact ID\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"phoneNumber\": {\n      \"type\": \"string\"\n    },\n    \"sentDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp in CST\"\n    },\n    \"clicks\": {\n      \"type\": \"integer\"\n    },\n    \"deliverability\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"delivered\",\n        \"failed\"\n      ]\n    },\n    \"replies\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\
  ,\n        \"properties\": {\n          \"message\": {\n            \"type\": \"string\"\n          },\n          \"date\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"Timestamp in CST\"\n          }\n        }\n      }\n    },\n    \"optOut\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"yes\",\n        \"no\"\n      ]\n    },\n    \"details\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"errorCode\": {\n          \"type\": \"string\"\n        },\n        \"errorSource\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"ac\",\n            \"twilio\"\n          ]\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/json-schema/activecampaign-sms-recipient-schema.json
tags:
- Marketing Automation
- Email Marketing
- CRM
- Sales Automation
- Customer Experience
title: Recipient
---
