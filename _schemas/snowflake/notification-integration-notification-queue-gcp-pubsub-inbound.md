---
description: ''
layout: schema
name: NotificationQueueGcpPubsubInbound
properties_list:
- description: Pub/Sub topic subscription ID used to allow Snowflake access to event messages.
  name: gcp_pubsub_subscription_name
  type: string
- description: Google Cloud Platform (GCP) service account created for your account.
  name: gcp_pubsub_service_account
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/notification-integration-notification-queue-gcp-pubsub-inbound-schema.json
slug: notification-integration-notification-queue-gcp-pubsub-inbound
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NotificationQueueGcpPubsubInbound\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"gcp_pubsub_subscription_name\": {\n      \"type\": \"string\",\n      \"description\": \"Pub/Sub topic subscription ID used to allow Snowflake access to event messages.\"\n    },\n    \"gcp_pubsub_service_account\": {\n      \"type\": \"string\",\n      \"description\": \"Google Cloud Platform (GCP) service account created for your account.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/notification-integration-notification-queue-gcp-pubsub-inbound-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: NotificationQueueGcpPubsubInbound
---
