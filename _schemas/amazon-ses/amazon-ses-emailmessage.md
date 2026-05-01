---
description: Schema for an Amazon SES email message object defining the content structure including simple, raw, and template-based email formats.
layout: schema
name: EmailMessage
properties_list:
- description: The simple email message with subject and body content.
  name: Simple
  type: object
- description: The raw email message in MIME format.
  name: Raw
  type: object
- description: The template-based email message.
  name: Template
  type: object
- description: The email address to use as the From address for the message.
  name: FromEmailAddress
  type: string
- description: The recipients of the email message.
  name: Destination
  type: object
- description: The reply-to email addresses for the message.
  name: ReplyToAddresses
  type: array
- description: The name of the configuration set to use when sending the email.
  name: ConfigurationSetName
  type: string
provider_name: Amazon SES
provider_slug: amazon-ses
schema_file: json-schema/amazon-ses-emailmessage-schema.json
slug: amazon-ses-emailmessage
source_filename: amazon-ses-emailmessage-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://aws.amazon.com/ses/schemas/emailmessage\",\n  \"title\": \"EmailMessage\",\n  \"description\": \"Schema for an Amazon SES email message object defining the content structure including simple, raw, and template-based email formats.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Simple\": {\n      \"type\": \"object\",\n      \"description\": \"The simple email message with subject and body content.\",\n      \"properties\": {\n        \"Subject\": {\n          \"type\": \"object\",\n          \"description\": \"The subject line of the email.\",\n          \"properties\": {\n            \"Data\": {\n              \"type\": \"string\",\n              \"description\": \"The content of the message subject.\"\n            },\n            \"Charset\": {\n              \"type\": \"string\",\n              \"description\": \"The character set for the subject content.\",\n              \"default\"\
  : \"UTF-8\"\n            }\n          },\n          \"required\": [\"Data\"]\n        },\n        \"Body\": {\n          \"type\": \"object\",\n          \"description\": \"The body of the email message.\",\n          \"properties\": {\n            \"Text\": {\n              \"type\": \"object\",\n              \"description\": \"The plain text body of the email.\",\n              \"properties\": {\n                \"Data\": {\n                  \"type\": \"string\",\n                  \"description\": \"The text content of the body.\"\n                },\n                \"Charset\": {\n                  \"type\": \"string\",\n                  \"description\": \"The character set for the text content.\",\n                  \"default\": \"UTF-8\"\n                }\n              },\n              \"required\": [\"Data\"]\n            },\n            \"Html\": {\n              \"type\": \"object\",\n              \"description\": \"The HTML body of the email.\",\n              \"properties\"\
  : {\n                \"Data\": {\n                  \"type\": \"string\",\n                  \"description\": \"The HTML content of the body.\"\n                },\n                \"Charset\": {\n                  \"type\": \"string\",\n                  \"description\": \"The character set for the HTML content.\",\n                  \"default\": \"UTF-8\"\n                }\n              },\n              \"required\": [\"Data\"]\n            }\n          }\n        }\n      },\n      \"required\": [\"Subject\", \"Body\"]\n    },\n    \"Raw\": {\n      \"type\": \"object\",\n      \"description\": \"The raw email message in MIME format.\",\n      \"properties\": {\n        \"Data\": {\n          \"type\": \"string\",\n          \"format\": \"byte\",\n          \"description\": \"The raw email message encoded in base64. The message must conform to MIME format.\"\n        }\n      },\n      \"required\": [\"Data\"]\n    },\n    \"Template\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"The template-based email message.\",\n      \"properties\": {\n        \"TemplateName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the email template to use.\"\n        },\n        \"TemplateArn\": {\n          \"type\": \"string\",\n          \"description\": \"The Amazon Resource Name (ARN) of the template.\"\n        },\n        \"TemplateData\": {\n          \"type\": \"string\",\n          \"description\": \"A JSON string of replacement values for template variables.\"\n        }\n      }\n    },\n    \"FromEmailAddress\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address to use as the From address for the message.\"\n    },\n    \"Destination\": {\n      \"type\": \"object\",\n      \"description\": \"The recipients of the email message.\",\n      \"properties\": {\n        \"ToAddresses\": {\n          \"type\": \"array\",\n          \"description\": \"An array of email addresses for the\
  \ To field.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"format\": \"email\"\n          }\n        },\n        \"CcAddresses\": {\n          \"type\": \"array\",\n          \"description\": \"An array of email addresses for the CC field.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"format\": \"email\"\n          }\n        },\n        \"BccAddresses\": {\n          \"type\": \"array\",\n          \"description\": \"An array of email addresses for the BCC field.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"format\": \"email\"\n          }\n        }\n      }\n    },\n    \"ReplyToAddresses\": {\n      \"type\": \"array\",\n      \"description\": \"The reply-to email addresses for the message.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"email\"\n      }\n    },\n    \"ConfigurationSetName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the\
  \ configuration set to use when sending the email.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ses/refs/heads/main/json-schema/amazon-ses-emailmessage-schema.json
tags:
- Email
- Email Deliverability
- Email Service
- Marketing Email
- Notifications
- SMTP
- Transactional Email
title: EmailMessage
---
