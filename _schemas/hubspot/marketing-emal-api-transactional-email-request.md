---
description: Request body for sending a transactional email
layout: schema
name: TransactionalEmailRequest
properties_list:
- description: The ID of the transactional email template to use
  name: emailId
  type: integer
- description: The email message configuration
  name: message
  type: object
- description: Properties to set on the contact (if createContact is enabled)
  name: contactProperties
  type: object
- description: Custom template variables for personalization
  name: customProperties
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/marketing-emal-api-transactional-email-request-schema.json
slug: marketing-emal-api-transactional-email-request
source_filename: marketing-emal-api-transactional-email-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/marketing-emal-api-transactional-email-request-schema.json\",\n  \"title\": \"TransactionalEmailRequest\",\n  \"description\": \"Request body for sending a transactional email\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"emailId\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the transactional email template to use\",\n      \"example\": 12345678\n    },\n    \"message\": {\n      \"type\": \"object\",\n      \"description\": \"The email message configuration\",\n      \"required\": [\n        \"to\"\n      ],\n      \"properties\": {\n        \"to\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"The recipient's email address\",\n          \"example\": \"recipient@example.com\"\n        },\n        \"from\": {\n          \"\
  type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"Override the from address (must be verified)\",\n          \"example\": \"noreply@yourcompany.com\"\n        },\n        \"sendId\": {\n          \"type\": \"string\",\n          \"description\": \"A unique ID to prevent duplicate sends\",\n          \"example\": \"unique-send-id-123\"\n        },\n        \"replyTo\": {\n          \"type\": \"array\",\n          \"description\": \"Reply-to email addresses\",\n          \"items\": {\n            \"type\": \"string\",\n            \"format\": \"email\"\n          },\n          \"example\": [\n            \"support@yourcompany.com\"\n          ]\n        },\n        \"cc\": {\n          \"type\": \"array\",\n          \"description\": \"CC email addresses\",\n          \"items\": {\n            \"type\": \"string\",\n            \"format\": \"email\"\n          },\n          \"example\": [\n            \"jsmith@example.com\"\n          ]\n        },\n   \
  \     \"bcc\": {\n          \"type\": \"array\",\n          \"description\": \"BCC email addresses\",\n          \"items\": {\n            \"type\": \"string\",\n            \"format\": \"email\"\n          },\n          \"example\": [\n            \"jsmith@example.com\"\n          ]\n        }\n      }\n    },\n    \"contactProperties\": {\n      \"type\": \"object\",\n      \"description\": \"Properties to set on the contact (if createContact is enabled)\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {\n        \"firstname\": \"John\",\n        \"lastname\": \"Doe\",\n        \"company\": \"Acme Corp\"\n      }\n    },\n    \"customProperties\": {\n      \"type\": \"object\",\n      \"description\": \"Custom template variables for personalization\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {\n        \"order_number\": \"ORD-12345\",\n        \"order_total\": \"$99.99\"\n      }\n\
  \    }\n  },\n  \"required\": [\n    \"emailId\",\n    \"message\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/marketing-emal-api-transactional-email-request-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: TransactionalEmailRequest
---
