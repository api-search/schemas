---
description: An email message archived in the Global Relay Archive, including headers, body content, recipients, and attachment references.
layout: schema
name: Global Relay Email
properties_list:
- description: Unique message identifier
  name: messageId
  type: string
- description: Sender of the email
  name: from
  type: object
- description: List of To recipients
  name: to
  type: array
- description: List of CC recipients
  name: cc
  type: array
- description: List of BCC recipients
  name: bcc
  type: array
- description: Email subject line
  name: subject
  type: string
- description: Date and time the email was sent
  name: sentDate
  type: string
- description: Date and time the email was received
  name: receivedDate
  type: string
- description: Email body content
  name: body
  type: object
- description: Email headers
  name: headers
  type: array
- description: IDs of attachments uploaded via /files endpoint
  name: attachmentIds
  type: array
provider_name: Global Relay
provider_slug: global-relay
schema_file: json-schema/global-relay-email.json
slug: global-relay-email
source_filename: global-relay-email.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"global-relay-email.json\",\n  \"title\": \"Global Relay Email\",\n  \"description\": \"An email message archived in the Global Relay Archive, including headers, body content, recipients, and attachment references.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"from\",\n    \"to\",\n    \"subject\",\n    \"sentDate\"\n  ],\n  \"properties\": {\n    \"messageId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique message identifier\"\n    },\n    \"from\": {\n      \"$ref\": \"global-relay-email-address.json\",\n      \"description\": \"Sender of the email\"\n    },\n    \"to\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"global-relay-email-address.json\"\n      },\n      \"description\": \"List of To recipients\"\n    },\n    \"cc\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"global-relay-email-address.json\"\n      },\n\
  \      \"description\": \"List of CC recipients\"\n    },\n    \"bcc\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"global-relay-email-address.json\"\n      },\n      \"description\": \"List of BCC recipients\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"Email subject line\"\n    },\n    \"sentDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the email was sent\"\n    },\n    \"receivedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the email was received\"\n    },\n    \"body\": {\n      \"type\": \"object\",\n      \"description\": \"Email body content\",\n      \"properties\": {\n        \"contentType\": {\n          \"type\": \"string\",\n          \"description\": \"MIME type of the body content\",\n          \"enum\": [\n            \"text/plain\",\n            \"text/html\"\n          ]\n\
  \        },\n        \"content\": {\n          \"type\": \"string\",\n          \"description\": \"Body content\"\n        }\n      }\n    },\n    \"headers\": {\n      \"type\": \"array\",\n      \"description\": \"Email headers\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Header name\"\n          },\n          \"value\": {\n            \"type\": \"string\",\n            \"description\": \"Header value\"\n          }\n        }\n      }\n    },\n    \"attachmentIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"IDs of attachments uploaded via /files endpoint\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/global-relay/refs/heads/main/json-schema/global-relay-email.json
tags:
- Archiving
- Compliance
- Data Retention
- Email Security
- Regulatory Compliance
title: Global Relay Email
---
