---
description: Configuration for envelope event notifications via DocuSign Connect webhooks.
layout: schema
name: EventNotification
properties_list:
- description: The webhook endpoint URL to receive notifications.
  name: url
  type: string
- description: When true, Connect logging is enabled.
  name: loggingEnabled
  type: string
- description: When true, requires HTTPS 200 acknowledgment.
  name: requireAcknowledgment
  type: string
- description: Envelope-level events to trigger notifications.
  name: envelopeEvents
  type: array
- description: Recipient-level events to trigger notifications.
  name: recipientEvents
  type: array
- description: When true, includes the certificate of completion.
  name: includeCertificateOfCompletion
  type: string
- description: When true, includes document PDFs in the notification.
  name: includeDocuments
  type: string
- description: When true, includes document custom fields.
  name: includeDocumentFields
  type: string
- description: When true, includes HMAC security headers.
  name: includeHMAC
  type: string
- description: ''
  name: includeSenderAccountAsCustomField
  type: string
- description: When true, includes time zone information.
  name: includeTimeZone
  type: string
- description: ''
  name: includeCertificateWithSoap
  type: string
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-event-notification-schema.json
slug: docusign-esignature-event-notification
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EventNotification\",\n  \"type\": \"object\",\n  \"description\": \"Configuration for envelope event notifications via DocuSign Connect webhooks.\",\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"The webhook endpoint URL to receive notifications.\"\n    },\n    \"loggingEnabled\": {\n      \"type\": \"string\",\n      \"description\": \"When true, Connect logging is enabled.\"\n    },\n    \"requireAcknowledgment\": {\n      \"type\": \"string\",\n      \"description\": \"When true, requires HTTPS 200 acknowledgment.\"\n    },\n    \"envelopeEvents\": {\n      \"type\": \"array\",\n      \"description\": \"Envelope-level events to trigger notifications.\"\n    },\n    \"recipientEvents\": {\n      \"type\": \"array\",\n      \"description\": \"Recipient-level events to trigger notifications.\"\n    },\n    \"includeCertificateOfCompletion\": {\n \
  \     \"type\": \"string\",\n      \"description\": \"When true, includes the certificate of completion.\"\n    },\n    \"includeDocuments\": {\n      \"type\": \"string\",\n      \"description\": \"When true, includes document PDFs in the notification.\"\n    },\n    \"includeDocumentFields\": {\n      \"type\": \"string\",\n      \"description\": \"When true, includes document custom fields.\"\n    },\n    \"includeHMAC\": {\n      \"type\": \"string\",\n      \"description\": \"When true, includes HMAC security headers.\"\n    },\n    \"includeSenderAccountAsCustomField\": {\n      \"type\": \"string\"\n    },\n    \"includeTimeZone\": {\n      \"type\": \"string\",\n      \"description\": \"When true, includes time zone information.\"\n    },\n    \"includeCertificateWithSoap\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-event-notification-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: EventNotification
---
