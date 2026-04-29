---
description: Response from a contact delete operation
layout: schema
name: DeleteContactResponse
properties_list:
- description: ''
  name: operationStatus
  type: string
- description: ''
  name: requestServiceMessageID
  type: string
- description: ''
  name: responseDateTime
  type: string
- description: Whether the asynchronous delete was successfully initiated
  name: operationInitiated
  type: boolean
provider_name: Salesforce Marketing Cloud
provider_slug: salesforce-marketing-cloud
schema_file: json-schema/salesforce-marketing-cloud-delete-contact-response-schema.json
slug: salesforce-marketing-cloud-delete-contact-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeleteContactResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response from a contact delete operation\",\n  \"properties\": {\n    \"operationStatus\": {\n      \"type\": \"string\"\n    },\n    \"requestServiceMessageID\": {\n      \"type\": \"string\"\n    },\n    \"responseDateTime\": {\n      \"type\": \"string\"\n    },\n    \"operationInitiated\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the asynchronous delete was successfully initiated\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/json-schema/salesforce-marketing-cloud-delete-contact-response-schema.json
tags:
- Automation
- Customer Journey
- Digital Marketing
- Email
- Marketing
- Personalization
title: DeleteContactResponse
---
