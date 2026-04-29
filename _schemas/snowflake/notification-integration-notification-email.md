---
description: ''
layout: schema
name: NotificationEmail
properties_list:
- description: A comma-separated list of quoted email addresses that can receive notification emails from this integration.
  name: allowed_recipients
  type: array
- description: A comma-separated list of default recipients for messages sent with this integration.
  name: default_recipients
  type: array
- description: the default subject line for messages sent with this integration.
  name: default_subject
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/notification-integration-notification-email-schema.json
slug: notification-integration-notification-email
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NotificationEmail\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowed_recipients\": {\n      \"type\": \"array\",\n      \"description\": \"A comma-separated list of quoted email addresses that can receive notification emails from this integration.\"\n    },\n    \"default_recipients\": {\n      \"type\": \"array\",\n      \"description\": \"A comma-separated list of default recipients for messages sent with this integration.\"\n    },\n    \"default_subject\": {\n      \"type\": \"string\",\n      \"description\": \"the default subject line for messages sent with this integration.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/notification-integration-notification-email-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: NotificationEmail
---
