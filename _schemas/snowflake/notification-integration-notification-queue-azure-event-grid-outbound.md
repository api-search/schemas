---
description: ''
layout: schema
name: NotificationQueueAzureEventGridOutbound
properties_list:
- description: Event Grid topic endpoint to which Snowpipe pushes notifications.
  name: azure_event_grid_topic_endpoint
  type: string
- description: ID of the Azure Active Directory tenant used for identity management.
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
schema_file: json-schema/notification-integration-notification-queue-azure-event-grid-outbound-schema.json
slug: notification-integration-notification-queue-azure-event-grid-outbound
source_filename: notification-integration-notification-queue-azure-event-grid-outbound-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NotificationQueueAzureEventGridOutbound\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"azure_event_grid_topic_endpoint\": {\n      \"type\": \"string\",\n      \"description\": \"Event Grid topic endpoint to which Snowpipe pushes notifications.\"\n    },\n    \"azure_tenant_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the Azure Active Directory tenant used for identity management.\"\n    },\n    \"azure_consent_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL to the Microsoft permissions request page.\"\n    },\n    \"azure_multi_tenant_app_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the Snowflake client application created for your account.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/notification-integration-notification-queue-azure-event-grid-outbound-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: NotificationQueueAzureEventGridOutbound
---
