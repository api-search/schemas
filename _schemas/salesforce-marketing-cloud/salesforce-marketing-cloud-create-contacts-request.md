---
description: Request body for creating one or more contacts
layout: schema
name: CreateContactsRequest
properties_list:
- description: Unique identifier for the contact
  name: contactKey
  type: string
- description: Attribute sets and values to assign to the contact
  name: attributeSets
  type: array
provider_name: Salesforce Marketing Cloud
provider_slug: salesforce-marketing-cloud
schema_file: json-schema/salesforce-marketing-cloud-create-contacts-request-schema.json
slug: salesforce-marketing-cloud-create-contacts-request
source_filename: salesforce-marketing-cloud-create-contacts-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateContactsRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating one or more contacts\",\n  \"properties\": {\n    \"contactKey\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the contact\"\n    },\n    \"attributeSets\": {\n      \"type\": \"array\",\n      \"description\": \"Attribute sets and values to assign to the contact\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/json-schema/salesforce-marketing-cloud-create-contacts-request-schema.json
tags:
- Automation
- Customer Journey
- Digital Marketing
- Email
- Marketing
- Personalization
title: CreateContactsRequest
---
