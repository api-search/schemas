---
description: Response returned after contact creation or update operations
layout: schema
name: ContactResponse
properties_list:
- description: Overall status of the operation
  name: operationStatus
  type: string
- description: Unique identifier for the request
  name: requestServiceMessageID
  type: string
- description: ''
  name: responseDateTime
  type: string
- description: ''
  name: resultMessages
  type: array
provider_name: Salesforce Marketing Cloud
provider_slug: salesforce-marketing-cloud
schema_file: json-schema/salesforce-marketing-cloud-contact-response-schema.json
slug: salesforce-marketing-cloud-contact-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContactResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response returned after contact creation or update operations\",\n  \"properties\": {\n    \"operationStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Overall status of the operation\"\n    },\n    \"requestServiceMessageID\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the request\"\n    },\n    \"responseDateTime\": {\n      \"type\": \"string\"\n    },\n    \"resultMessages\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/json-schema/salesforce-marketing-cloud-contact-response-schema.json
tags:
- Automation
- Customer Journey
- Digital Marketing
- Email
- Marketing
- Personalization
title: ContactResponse
---
