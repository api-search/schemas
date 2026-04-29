---
description: Custom email notification settings for a recipient.
layout: schema
name: RecipientEmailNotification
properties_list:
- description: Custom email subject for this recipient.
  name: emailSubject
  type: string
- description: Custom email body for this recipient.
  name: emailBody
  type: string
- description: Language code for the notification.
  name: supportedLanguage
  type: string
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-recipient-email-notification-schema.json
slug: docusign-esignature-recipient-email-notification
source_filename: docusign-esignature-recipient-email-notification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RecipientEmailNotification\",\n  \"type\": \"object\",\n  \"description\": \"Custom email notification settings for a recipient.\",\n  \"properties\": {\n    \"emailSubject\": {\n      \"type\": \"string\",\n      \"description\": \"Custom email subject for this recipient.\"\n    },\n    \"emailBody\": {\n      \"type\": \"string\",\n      \"description\": \"Custom email body for this recipient.\"\n    },\n    \"supportedLanguage\": {\n      \"type\": \"string\",\n      \"description\": \"Language code for the notification.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-recipient-email-notification-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: RecipientEmailNotification
---
