---
description: ''
layout: schema
name: NotificationQueueGcpPubsubOutbound
properties_list:
- description: Identification of the Pub/Sub topic to which Snowpipe pushes notifications.
  name: gcp_pubsub_topic_name
  type: string
- description: Google Cloud Platform (GCP) service account created for your account.
  name: gcp_pubsub_service_account
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/notification-integration-notification-queue-gcp-pubsub-outbound-schema.json
slug: notification-integration-notification-queue-gcp-pubsub-outbound
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NotificationQueueGcpPubsubOutbound\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"gcp_pubsub_topic_name\": {\n      \"type\": \"string\",\n      \"description\": \"Identification of the Pub/Sub topic to which Snowpipe pushes notifications.\"\n    },\n    \"gcp_pubsub_service_account\": {\n      \"type\": \"string\",\n      \"description\": \"Google Cloud Platform (GCP) service account created for your account.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/notification-integration-notification-queue-gcp-pubsub-outbound-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: NotificationQueueGcpPubsubOutbound
---
