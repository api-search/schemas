---
description: Information about a Mandrill template.
layout: schema
name: TemplateInfo
properties_list:
- description: The URL-safe slug for the template.
  name: slug
  type: string
- description: The display name of the template.
  name: name
  type: string
- description: Labels applied to the template for organization.
  name: labels
  type: array
- description: The HTML code of the template.
  name: code
  type: string
- description: The default subject line.
  name: subject
  type: string
- description: The default from address.
  name: from_email
  type: string
- description: The default from name.
  name: from_name
  type: string
- description: The default text content.
  name: text
  type: string
- description: The name of the published version.
  name: publish_name
  type: string
- description: The HTML code of the published version.
  name: publish_code
  type: string
- description: The subject of the published version.
  name: publish_subject
  type: string
- description: The from address of the published version.
  name: publish_from_email
  type: string
- description: The from name of the published version.
  name: publish_from_name
  type: string
- description: The text content of the published version.
  name: publish_text
  type: string
- description: When the template was last published.
  name: published_at
  type: string
- description: When the template was created.
  name: created_at
  type: string
- description: When the template was last updated.
  name: updated_at
  type: string
provider_name: Mailchimp
provider_slug: mailchimp
schema_file: json-schema/mailchimp-transactional-template-info-schema.json
slug: mailchimp-transactional-template-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TemplateInfo\",\n  \"type\": \"object\",\n  \"description\": \"Information about a Mandrill template.\",\n  \"properties\": {\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"The URL-safe slug for the template.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the template.\"\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"description\": \"Labels applied to the template for organization.\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"The HTML code of the template.\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"The default subject line.\"\n    },\n    \"from_email\": {\n      \"type\": \"string\",\n      \"description\": \"The default from address.\"\n    },\n    \"from_name\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The default from name.\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"The default text content.\"\n    },\n    \"publish_name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the published version.\"\n    },\n    \"publish_code\": {\n      \"type\": \"string\",\n      \"description\": \"The HTML code of the published version.\"\n    },\n    \"publish_subject\": {\n      \"type\": \"string\",\n      \"description\": \"The subject of the published version.\"\n    },\n    \"publish_from_email\": {\n      \"type\": \"string\",\n      \"description\": \"The from address of the published version.\"\n    },\n    \"publish_from_name\": {\n      \"type\": \"string\",\n      \"description\": \"The from name of the published version.\"\n    },\n    \"publish_text\": {\n      \"type\": \"string\",\n      \"description\": \"The text content of the published version.\"\n    },\n    \"published_at\": {\n      \"type\": \"string\",\n      \"\
  description\": \"When the template was last published.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the template was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the template was last updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/json-schema/mailchimp-transactional-template-info-schema.json
tags:
- Campaigns
- Email Marketing
- Marketing Automation
- Newsletters
- Transactional Email
title: TemplateInfo
---
