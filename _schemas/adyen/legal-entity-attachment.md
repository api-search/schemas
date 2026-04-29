---
description: Attachment schema from Adyen API
layout: schema
name: Attachment
properties_list:
- description: The document in Base64-encoded string format.
  name: content
  type: string
- description: 'The file format. Possible values: **application/pdf**, **image/jpg**, **image/jpeg**, **image/png**.'
  name: contentType
  type: string
- description: The name of the file including the file extension.
  name: filename
  type: string
- description: The name of the file including the file extension.
  name: pageName
  type: string
- description: Specifies which side of the ID card is uploaded. * When `type` is **driversLicense** or **identityCard**, set this to **front** or **back**. * When omitted, we infer the page number based on the order
  name: pageType
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-attachment-schema.json
slug: legal-entity-attachment
source_filename: legal-entity-attachment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-attachment-schema.json\",\n  \"title\": \"Attachment\",\n  \"description\": \"Attachment schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content\": {\n      \"description\": \"The document in Base64-encoded string format.\",\n      \"format\": \"byte\",\n      \"type\": \"string\"\n    },\n    \"contentType\": {\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"1\",\n      \"description\": \"The file format.\\n\\n Possible values: **application/pdf**, **image/jpg**, **image/jpeg**, **image/png**. \",\n      \"type\": \"string\"\n    },\n    \"filename\": {\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"1\",\n      \"description\": \"The name of the file including the file extension.\",\n      \"type\": \"string\"\n    },\n    \"pageName\"\
  : {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The name of the file including the file extension.\",\n      \"type\": \"string\"\n    },\n    \"pageType\": {\n      \"description\": \"Specifies which side of the ID card is uploaded.\\n\\n* When `type` is **driversLicense** or **identityCard**, set this to **front** or **back**.\\n\\n* When omitted, we infer the page number based on the order of attachments.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"content\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-attachment-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Attachment
---
