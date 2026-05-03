---
description: Normalized contact entity returned by the Revert Unified CRM API across Salesforce, HubSpot, Zoho CRM, Pipedrive, and Close CRM
layout: schema
name: Revert Unified CRM Contact
properties_list:
- description: Revert-normalized unique contact identifier
  name: id
  type: string
- description: The original ID from the source CRM provider
  name: remoteId
  type: string
- description: Contact's first name
  name: firstName
  type: string
- description: Contact's last name
  name: lastName
  type: string
- description: Primary email address
  name: email
  type: string
- description: Primary phone number
  name: phone
  type: string
- description: Associated company name
  name: company
  type: string
- description: Job title
  name: title
  type: string
- description: Record creation timestamp
  name: createdAt
  type: string
- description: Record last update timestamp
  name: updatedAt
  type: string
- description: Non-unified fields from the source CRM provider
  name: additional
  type: object
provider_name: Revert
provider_slug: revert
schema_file: json-schema/revert-contact-schema.json
slug: revert-contact
source_filename: revert-contact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/revert/main/json-schema/revert-contact-schema.json\",\n  \"title\": \"Revert Unified CRM Contact\",\n  \"description\": \"Normalized contact entity returned by the Revert Unified CRM API across Salesforce, HubSpot, Zoho CRM, Pipedrive, and Close CRM\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Revert-normalized unique contact identifier\"\n    },\n    \"remoteId\": {\n      \"type\": \"string\",\n      \"description\": \"The original ID from the source CRM provider\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"Contact's first name\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"Contact's last name\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\"\
  : \"Primary email address\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"Primary phone number\"\n    },\n    \"company\": {\n      \"type\": \"string\",\n      \"description\": \"Associated company name\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Job title\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record creation timestamp\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record last update timestamp\"\n    },\n    \"additional\": {\n      \"type\": \"object\",\n      \"description\": \"Non-unified fields from the source CRM provider\"\n    }\n  },\n  \"required\": [\"id\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/json-schema/revert-contact-schema.json
tags:
- Integrations
- CRM
- Unified API
- Open Source
title: Revert Unified CRM Contact
---
