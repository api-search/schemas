---
description: ''
layout: schema
name: NotificationQueueAzureEventGridInbound
properties_list:
- description: the queue ID for the Azure Queue Storage queue created for Event Grid notifications.
  name: azure_storage_queue_primary_uri
  type: string
- description: the ID of the Azure Active Directory tenant used for identity management.
  name: azure_tenant_id
  type: string
- description: URL to the Microsoft permissions request page.
  name: azure_consent_url
  type: string
- description: Name of the Snowflake client application created for your account.
  name: azure_multi_tenant_app_name
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/notification-integration-notification-queue-azure-event-grid-inbound-schema.json
slug: notification-integration-notification-queue-azure-event-grid-inbound
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NotificationQueueAzureEventGridInbound\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"azure_storage_queue_primary_uri\": {\n      \"type\": \"string\",\n      \"description\": \"the queue ID for the Azure Queue Storage queue created for Event Grid notifications.\"\n    },\n    \"azure_tenant_id\": {\n      \"type\": \"string\",\n      \"description\": \"the ID of the Azure Active Directory tenant used for identity management.\"\n    },\n    \"azure_consent_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL to the Microsoft permissions request page.\"\n    },\n    \"azure_multi_tenant_app_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the Snowflake client application created for your account.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/notification-integration-notification-queue-azure-event-grid-inbound-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: NotificationQueueAzureEventGridInbound
---
