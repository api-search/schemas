---
description: An email recipient for report delivery.
layout: schema
name: Recipient
properties_list:
- description: The email address of the recipient.
  name: email
  type: string
- description: The delivery type for this recipient.
  name: deliveryType
  type: string
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-recipient-schema.json
slug: google-campaign-manager-recipient
source_filename: google-campaign-manager-recipient-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Recipient\",\n  \"type\": \"object\",\n  \"description\": \"An email recipient for report delivery.\",\n  \"properties\": {\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"The email address of the recipient.\"\n    },\n    \"deliveryType\": {\n      \"type\": \"string\",\n      \"description\": \"The delivery type for this recipient.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-recipient-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: Recipient
---
