---
description: Envelope notification settings including reminders and expirations.
layout: schema
name: Notification
properties_list:
- description: When true, use account default notification settings.
  name: useAccountDefaults
  type: string
- description: ''
  name: reminders
  type: object
- description: ''
  name: expirations
  type: object
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-notification-schema.json
slug: docusign-esignature-notification
source_filename: docusign-esignature-notification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Notification\",\n  \"type\": \"object\",\n  \"description\": \"Envelope notification settings including reminders and expirations.\",\n  \"properties\": {\n    \"useAccountDefaults\": {\n      \"type\": \"string\",\n      \"description\": \"When true, use account default notification settings.\"\n    },\n    \"reminders\": {\n      \"type\": \"object\"\n    },\n    \"expirations\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-notification-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: Notification
---
