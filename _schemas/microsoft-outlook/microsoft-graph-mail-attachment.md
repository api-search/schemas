---
description: Base resource for file, item, and reference attachments. Use the @odata.type property to specify the derived type.
layout: schema
name: Attachment
properties_list:
- description: 'The OData type of the attachment. Use #microsoft.graph.fileAttachment for file attachments or #microsoft.graph.itemAttachment for item attachments.'
  name: '@odata.type'
  type: string
- description: The unique identifier of the attachment. Read-only.
  name: id
  type: string
- description: The display name of the attachment.
  name: name
  type: string
- description: The MIME type of the attachment.
  name: contentType
  type: string
- description: The length of the attachment in bytes.
  name: size
  type: integer
- description: True if the attachment is an inline attachment.
  name: isInline
  type: boolean
- description: The date and time the attachment was last modified in UTC.
  name: lastModifiedDateTime
  type: string
- description: The base64-encoded contents of the file. Only applicable for fileAttachment.
  name: contentBytes
  type: string
- description: The ID of the attachment in the Exchange store. Only applicable for fileAttachment.
  name: contentId
  type: string
- description: The Uniform Resource Identifier (URI) corresponding to the location of the content of the attachment.
  name: contentLocation
  type: string
provider_name: Microsoft Outlook
provider_slug: microsoft-outlook
schema_file: json-schema/microsoft-graph-mail-attachment-schema.json
slug: microsoft-graph-mail-attachment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Attachment\",\n  \"type\": \"object\",\n  \"description\": \"Base resource for file, item, and reference attachments. Use the @odata.type property to specify the derived type.\",\n  \"properties\": {\n    \"@odata.type\": {\n      \"type\": \"string\",\n      \"description\": \"The OData type of the attachment. Use #microsoft.graph.fileAttachment for file attachments or #microsoft.graph.itemAttachment for item attachments.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the attachment. Read-only.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the attachment.\"\n    },\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"The MIME type of the attachment.\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"The length of the attachment\
  \ in bytes.\"\n    },\n    \"isInline\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the attachment is an inline attachment.\"\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the attachment was last modified in UTC.\"\n    },\n    \"contentBytes\": {\n      \"type\": \"string\",\n      \"description\": \"The base64-encoded contents of the file. Only applicable for fileAttachment.\"\n    },\n    \"contentId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the attachment in the Exchange store. Only applicable for fileAttachment.\"\n    },\n    \"contentLocation\": {\n      \"type\": \"string\",\n      \"description\": \"The Uniform Resource Identifier (URI) corresponding to the location of the content of the attachment.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-outlook/refs/heads/main/json-schema/microsoft-graph-mail-attachment-schema.json
tags:
- Calendar
- Contacts
- Email
- Enterprise
- Microsoft
- Office 365
- Productivity
title: Attachment
---
