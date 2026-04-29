---
description: A Mailchimp email template. Templates are reusable email layouts that can be used across campaigns. They can be user-created, base templates provided by Mailchimp, or gallery templates. Templates support drag-and-drop editing, responsive design, and custom HTML.
layout: schema
name: Mailchimp Template
properties_list:
- description: The individual ID for the template.
  name: id
  type: integer
- description: The type of template (user, base, or gallery).
  name: type
  type: string
- description: The name of the template.
  name: name
  type: string
- description: Whether the template uses the drag and drop editor.
  name: drag_and_drop
  type: boolean
- description: Whether the template contains media queries to make it responsive.
  name: responsive
  type: boolean
- description: If available, the category the template is listed in.
  name: category
  type: string
- description: The date and time the template was created in ISO 8601 format.
  name: date_created
  type: string
- description: The date and time the template was edited in ISO 8601 format.
  name: date_edited
  type: string
- description: The login name of the template's creator.
  name: created_by
  type: string
- description: The login name of who last edited the template.
  name: edited_by
  type: string
- description: User templates are not deleted but rather marked as inactive. Returns whether the template is still active.
  name: active
  type: boolean
- description: The ID of the folder the template is currently in.
  name: folder_id
  type: string
- description: If available, the URL for a thumbnail of the template.
  name: thumbnail
  type: string
- description: The URL used for template sharing.
  name: share_url
  type: string
- description: How the template's content is put together. 'template' for legacy editor, 'multichannel' for new editor, 'html' for code-your-own.
  name: content_type
  type: string
- description: The raw HTML source of the template. Available when fetching individual template content.
  name: html
  type: string
- description: A dictionary of content sections within the template. Keys are section names, values are the HTML content. Only available for templates with editable content areas.
  name: sections
  type: object
provider_name: Mailchimp
provider_slug: mailchimp
schema_file: json-schema/template.json
slug: template
source_filename: template.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/messaging/mailchimp/json-schema/template.json\",\n  \"title\": \"Mailchimp Template\",\n  \"description\": \"A Mailchimp email template. Templates are reusable email layouts that can be used across campaigns. They can be user-created, base templates provided by Mailchimp, or gallery templates. Templates support drag-and-drop editing, responsive design, and custom HTML.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The individual ID for the template.\",\n      \"readOnly\": true\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of template (user, base, or gallery).\",\n      \"enum\": [\"user\", \"base\", \"gallery\"],\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the template.\"\n \
  \   },\n    \"drag_and_drop\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the template uses the drag and drop editor.\",\n      \"readOnly\": true\n    },\n    \"responsive\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the template contains media queries to make it responsive.\",\n      \"readOnly\": true\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"If available, the category the template is listed in.\",\n      \"readOnly\": true\n    },\n    \"date_created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the template was created in ISO 8601 format.\",\n      \"readOnly\": true\n    },\n    \"date_edited\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the template was edited in ISO 8601 format.\",\n      \"readOnly\": true\n    },\n    \"created_by\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The login name of the template's creator.\",\n      \"readOnly\": true\n    },\n    \"edited_by\": {\n      \"type\": \"string\",\n      \"description\": \"The login name of who last edited the template.\",\n      \"readOnly\": true\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"User templates are not deleted but rather marked as inactive. Returns whether the template is still active.\",\n      \"readOnly\": true\n    },\n    \"folder_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the folder the template is currently in.\"\n    },\n    \"thumbnail\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"If available, the URL for a thumbnail of the template.\",\n      \"readOnly\": true\n    },\n    \"share_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL used for template sharing.\",\n      \"readOnly\": true\n    },\n\
  \    \"content_type\": {\n      \"type\": \"string\",\n      \"description\": \"How the template's content is put together. 'template' for legacy editor, 'multichannel' for new editor, 'html' for code-your-own.\",\n      \"enum\": [\"template\", \"multichannel\", \"html\"],\n      \"readOnly\": true\n    },\n    \"html\": {\n      \"type\": \"string\",\n      \"description\": \"The raw HTML source of the template. Available when fetching individual template content.\"\n    },\n    \"sections\": {\n      \"type\": \"object\",\n      \"description\": \"A dictionary of content sections within the template. Keys are section names, values are the HTML content. Only available for templates with editable content areas.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\"name\"],\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/json-schema/template.json
tags:
- Campaigns
- Email Marketing
- Marketing Automation
- Newsletters
- Transactional Email
title: Mailchimp Template
---
