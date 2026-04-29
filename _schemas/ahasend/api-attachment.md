---
description: Attachment schema from AhaSend API
layout: schema
name: Attachment
properties_list:
- description: The attachment data. If the base64 field is true, this data must be encoded using base64. Otherwise, it will be interpreted as UTF-8.
  name: data
  type: string
- description: If set to true, data needs to be encoded using base64. Otherwise data will be interpreted as UTF-8.
  name: base64
  type: boolean
- description: ''
  name: content_type
  type: string
- description: If specified, this attachment will be added as an inline attachment and a multipart/related MIME container will be generated in the message to hold it and the textual content.
  name: content_id
  type: string
- description: ''
  name: file_name
  type: string
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/api-attachment-schema.json
slug: api-attachment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/api-attachment-schema.json\",\n  \"title\": \"Attachment\",\n  \"description\": \"Attachment schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"string\",\n      \"examples\": [\n        \"R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7\"\n      ],\n      \"description\": \"The attachment data. If the base64 field is true, this data must be encoded using base64. Otherwise, it will be interpreted as UTF-8.\",\n      \"example\": \"example_value\"\n    },\n    \"base64\": {\n      \"type\": \"boolean\",\n      \"examples\": [\n        true,\n        false\n      ],\n      \"description\": \"If set to true, data needs to be encoded using base64. Otherwise data will be interpreted as UTF-8.\",\n      \"example\": true\n    },\n    \"content_type\":\
  \ {\n      \"type\": \"string\",\n      \"examples\": [\n        \"image/gif\"\n      ],\n      \"example\": \"example_value\"\n    },\n    \"content_id\": {\n      \"type\": \"string\",\n      \"examples\": [\n        \"my-image\"\n      ],\n      \"description\": \"If specified, this attachment will be added as an inline attachment and a multipart/related MIME container will be generated in the message to hold it and the textual content.\",\n      \"example\": \"500123\"\n    },\n    \"file_name\": {\n      \"type\": \"string\",\n      \"examples\": [\n        \"my_image.gif\"\n      ],\n      \"example\": \"Example Name\"\n    }\n  },\n  \"required\": [\n    \"data\",\n    \"file_name\",\n    \"content_type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/api-attachment-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: Attachment
---
