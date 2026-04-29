---
description: An object that defines the email message content including simple, raw, and template options.
layout: schema
name: EmailMessage
properties_list:
- description: The simple email message with subject and body.
  name: Simple
  type: object
- description: The raw email message.
  name: Raw
  type: object
- description: The template email message.
  name: Template
  type: object
provider_name: Amazon SES
provider_slug: amazon-ses
schema_file: json-schema/amazon-ses-openapi-email-message-schema.json
slug: amazon-ses-openapi-email-message
source_filename: amazon-ses-openapi-email-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ses/refs/heads/main/json-schema/amazon-ses-openapi-email-message-schema.json\",\n  \"title\": \"EmailMessage\",\n  \"description\": \"An object that defines the email message content including simple, raw, and template options.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Simple\": {\n      \"type\": \"object\",\n      \"description\": \"The simple email message with subject and body.\",\n      \"properties\": {\n        \"Subject\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"Data\": {\n              \"type\": \"string\",\n              \"description\": \"The content of the message subject.\"\n            },\n            \"Charset\": {\n              \"type\": \"string\",\n              \"description\": \"The character set for the content.\"\n            }\n          },\n          \"required\"\
  : [\n            \"Data\"\n          ]\n        },\n        \"Body\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"Text\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"Data\": {\n                  \"type\": \"string\"\n                },\n                \"Charset\": {\n                  \"type\": \"string\"\n                }\n              },\n              \"required\": [\n                \"Data\"\n              ]\n            },\n            \"Html\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"Data\": {\n                  \"type\": \"string\"\n                },\n                \"Charset\": {\n                  \"type\": \"string\"\n                }\n              },\n              \"required\": [\n                \"Data\"\n              ]\n            }\n          }\n        }\n      },\n      \"required\": [\n        \"Subject\",\n        \"Body\"\n  \
  \    ]\n    },\n    \"Raw\": {\n      \"type\": \"object\",\n      \"description\": \"The raw email message.\",\n      \"properties\": {\n        \"Data\": {\n          \"type\": \"string\",\n          \"format\": \"byte\",\n          \"description\": \"The raw email message in MIME format.\"\n        }\n      },\n      \"required\": [\n        \"Data\"\n      ]\n    },\n    \"Template\": {\n      \"type\": \"object\",\n      \"description\": \"The template email message.\",\n      \"properties\": {\n        \"TemplateName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the template.\"\n        },\n        \"TemplateArn\": {\n          \"type\": \"string\"\n        },\n        \"TemplateData\": {\n          \"type\": \"string\",\n          \"description\": \"JSON object of replacement values for template variables.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ses/refs/heads/main/json-schema/amazon-ses-openapi-email-message-schema.json
tags:
- AWS
- Email
- Email Deliverability
- Email Service
- Marketing Email
- Notifications
- SMTP
- Transactional Email
title: EmailMessage
---
