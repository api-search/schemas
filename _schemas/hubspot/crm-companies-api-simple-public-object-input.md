---
description: Input for creating or updating a CRM object.
layout: schema
name: SimplePublicObjectInput
properties_list:
- description: The properties to set on the object.
  name: properties
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/crm-companies-api-simple-public-object-input-schema.json
slug: crm-companies-api-simple-public-object-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-companies-api-simple-public-object-input-schema.json\",\n  \"title\": \"SimplePublicObjectInput\",\n  \"description\": \"Input for creating or updating a CRM object.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"The properties to set on the object.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-companies-api-simple-public-object-input-schema.json
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
title: SimplePublicObjectInput
---
