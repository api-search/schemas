---
description: Represents the upload session for iterative file upload.
layout: schema
name: UploadSession
properties_list:
- description: The URL endpoint that accepts PUT requests for byte ranges of the file.
  name: uploadUrl
  type: string
- description: The date and time in UTC that the upload session will expire.
  name: expirationDateTime
  type: string
- description: A collection of byte ranges that the server is missing for the file, such as "0-25", "128-500".
  name: nextExpectedRanges
  type: array
provider_name: Microsoft Outlook
provider_slug: microsoft-outlook
schema_file: json-schema/microsoft-graph-mail-upload-session-schema.json
slug: microsoft-graph-mail-upload-session
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UploadSession\",\n  \"type\": \"object\",\n  \"description\": \"Represents the upload session for iterative file upload.\",\n  \"properties\": {\n    \"uploadUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The URL endpoint that accepts PUT requests for byte ranges of the file.\"\n    },\n    \"expirationDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time in UTC that the upload session will expire.\"\n    },\n    \"nextExpectedRanges\": {\n      \"type\": \"array\",\n      \"description\": \"A collection of byte ranges that the server is missing for the file, such as \\\"0-25\\\", \\\"128-500\\\".\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-outlook/refs/heads/main/json-schema/microsoft-graph-mail-upload-session-schema.json
tags:
- Calendar
- Contacts
- Email
- Enterprise
- Microsoft
- Office 365
- Productivity
title: UploadSession
---
