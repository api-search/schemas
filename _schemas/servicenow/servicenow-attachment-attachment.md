---
description: Metadata about a file attachment stored in ServiceNow.
layout: schema
name: Attachment
properties_list:
- description: Unique identifier for the attachment record.
  name: sys_id
  type: string
- description: The name of the attached file.
  name: file_name
  type: string
- description: The table to which the attachment belongs.
  name: table_name
  type: string
- description: The sys_id of the record to which the file is attached.
  name: table_sys_id
  type: string
- description: The MIME type of the attached file.
  name: content_type
  type: string
- description: The size of the attached file in bytes.
  name: size_bytes
  type: integer
- description: The compressed size of the attached file in bytes.
  name: size_compressed
  type: integer
- description: The URL to download the attachment file content.
  name: download_link
  type: string
- description: The height in pixels if the attachment is an image.
  name: image_height
  type: integer
- description: The width in pixels if the attachment is an image.
  name: image_width
  type: integer
- description: The MD5 hash of the file content.
  name: hash
  type: string
- description: The state of the attachment processing.
  name: state
  type: string
- description: The date and time the attachment was created.
  name: sys_created_on
  type: string
- description: The user who uploaded the attachment.
  name: sys_created_by
  type: string
- description: The date and time the attachment was last modified.
  name: sys_updated_on
  type: string
- description: The user who last modified the attachment record.
  name: sys_updated_by
  type: string
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/servicenow-attachment-attachment-schema.json
slug: servicenow-attachment-attachment
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Metadata about a file attachment stored in ServiceNow.\",\n  \"properties\": {\n    \"sys_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the attachment record.\",\n      \"example\": \"500123\"\n    },\n    \"file_name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the attached file.\",\n      \"example\": \"example_value\"\n    },\n    \"table_name\": {\n      \"type\": \"string\",\n      \"description\": \"The table to which the attachment belongs.\",\n      \"example\": \"example_value\"\n    },\n    \"table_sys_id\": {\n      \"type\": \"string\",\n      \"description\": \"The sys_id of the record to which the file is attached.\",\n      \"example\": \"500123\"\n    },\n    \"content_type\": {\n      \"type\": \"string\",\n      \"description\": \"The MIME type of the attached file.\",\n      \"example\": \"example_value\"\n    },\n    \"size_bytes\": {\n    \
  \  \"type\": \"integer\",\n      \"description\": \"The size of the attached file in bytes.\",\n      \"example\": 10\n    },\n    \"size_compressed\": {\n      \"type\": \"integer\",\n      \"description\": \"The compressed size of the attached file in bytes.\",\n      \"example\": 10\n    },\n    \"download_link\": {\n      \"type\": \"string\",\n      \"description\": \"The URL to download the attachment file content.\",\n      \"format\": \"uri\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"image_height\": {\n      \"type\": \"integer\",\n      \"description\": \"The height in pixels if the attachment is an image.\",\n      \"example\": 10\n    },\n    \"image_width\": {\n      \"type\": \"integer\",\n      \"description\": \"The width in pixels if the attachment is an image.\",\n      \"example\": 10\n    },\n    \"hash\": {\n      \"type\": \"string\",\n      \"description\": \"The MD5 hash of the file content.\",\n      \"example\": \"example_value\"\n    },\n\
  \    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The state of the attachment processing.\",\n      \"example\": \"example_value\"\n    },\n    \"sys_created_on\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the attachment was created.\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"sys_created_by\": {\n      \"type\": \"string\",\n      \"description\": \"The user who uploaded the attachment.\",\n      \"example\": \"example_value\"\n    },\n    \"sys_updated_on\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the attachment was last modified.\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"sys_updated_by\": {\n      \"type\": \"string\",\n      \"description\": \"The user who last modified the attachment record.\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"Attachment\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/servicenow-attachment-attachment-schema.json
tags:
- Automation
- Cloud Services
- Digital Workflows
- Enterprise Platform
- IT Service Management
- ITSM
- Processes
- T1
- Workflow Automation
- Workflows
title: Attachment
---
