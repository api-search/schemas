---
description: Represents a content control in a Word document.
layout: schema
name: ContentControl
properties_list:
- description: Unique identifier of the content control.
  name: id
  type: string
- description: Tag to identify the content control.
  name: tag
  type: string
- description: Title of the content control.
  name: title
  type: string
- description: Type of content control.
  name: type
  type: string
- description: Text content of the content control.
  name: text
  type: string
- description: Visual appearance.
  name: appearance
  type: string
- description: Whether the content control can be deleted.
  name: cannotDelete
  type: boolean
- description: Whether the content control can be edited.
  name: cannotEdit
  type: boolean
provider_name: Microsoft Word
provider_slug: microsoft-word
schema_file: json-schema/javascript-api-content-control-schema.json
slug: javascript-api-content-control
source_filename: javascript-api-content-control-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/json-schema/javascript-api-content-control-schema.json\",\n  \"title\": \"ContentControl\",\n  \"description\": \"Represents a content control in a Word document.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the content control.\"\n    },\n    \"tag\": {\n      \"type\": \"string\",\n      \"description\": \"Tag to identify the content control.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the content control.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of content control.\",\n      \"enum\": [\"RichText\", \"PlainText\", \"Picture\", \"CheckBox\", \"DropDownList\", \"ComboBox\", \"DatePicker\"]\n    },\n    \"text\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Text content of the content control.\"\n    },\n    \"appearance\": {\n      \"type\": \"string\",\n      \"description\": \"Visual appearance.\",\n      \"enum\": [\"BoundingBox\", \"Tags\", \"Hidden\"]\n    },\n    \"cannotDelete\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the content control can be deleted.\"\n    },\n    \"cannotEdit\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the content control can be edited.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/json-schema/javascript-api-content-control-schema.json
tags:
- Documents
- Microsoft 365
- Office
- Productivity
- Word Processing
title: ContentControl
---
