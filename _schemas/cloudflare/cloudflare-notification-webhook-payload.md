---
description: The standard payload structure for Cloudflare notification webhooks. When an alert fires, Cloudflare sends an HTTP POST with this JSON payload to configured webhook endpoints.
layout: schema
name: Cloudflare Notification Webhook Payload
properties_list:
- description: The name of the notification policy that triggered this webhook.
  name: name
  type: string
- description: Human-readable description of the alert with interpolated values specific to the event.
  name: text
  type: string
- description: Alert-specific data whose structure varies depending on the alert_type. Contains detailed information about the event that triggered the notification.
  name: data
  type: object
- description: Unix timestamp in seconds when the notification was generated.
  name: ts
  type: integer
- description: The Cloudflare account identifier associated with the notification. May not be present in all notifications.
  name: account_id
  type: string
- description: The UUID of the notification policy that triggered the webhook.
  name: policy_id
  type: string
- description: The name of the notification policy.
  name: policy_name
  type: string
- description: The unique identifier for the alert category (e.g., advanced_ddos_attack_l4_alert, health_check_status_notification).
  name: alert_type
  type: string
- description: UUID for grouping related alerts that are part of the same incident.
  name: alert_correlation_id
  type: string
- description: The event state indicating whether the alert is starting or ending.
  name: alert_event
  type: string
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-notification-webhook-payload-schema.json
slug: cloudflare-notification-webhook-payload
source_filename: cloudflare-notification-webhook-payload-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-notification-webhook-payload-schema.json\",\n  \"title\": \"Cloudflare Notification Webhook Payload\",\n  \"description\": \"The standard payload structure for Cloudflare notification webhooks. When an alert fires, Cloudflare sends an HTTP POST with this JSON payload to configured webhook endpoints.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"text\", \"data\", \"ts\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the notification policy that triggered this webhook.\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the alert with interpolated values specific to the event.\"\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"Alert-specific\
  \ data whose structure varies depending on the alert_type. Contains detailed information about the event that triggered the notification.\"\n    },\n    \"ts\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp in seconds when the notification was generated.\"\n    },\n    \"account_id\": {\n      \"type\": \"string\",\n      \"description\": \"The Cloudflare account identifier associated with the notification. May not be present in all notifications.\"\n    },\n    \"policy_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The UUID of the notification policy that triggered the webhook.\"\n    },\n    \"policy_name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the notification policy.\"\n    },\n    \"alert_type\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the alert category (e.g., advanced_ddos_attack_l4_alert, health_check_status_notification).\",\n    \
  \  \"enum\": [\n        \"advanced_ddos_attack_l4_alert\",\n        \"advanced_ddos_attack_l7_alert\",\n        \"dedicated_ssl_certificate_event_type\",\n        \"health_check_status_notification\",\n        \"workers_alert\",\n        \"workers_observability_alert\",\n        \"access_custom_certificate_expiration_type\",\n        \"zone_aop_custom_certificate_expiration_type\",\n        \"universal_ssl_event_type\",\n        \"clickhouse_alert_fw_anomaly\",\n        \"clickhouse_alert_fw_ent_anomaly\",\n        \"real_origin_monitoring\",\n        \"failing_logpush_job_disabled_alert\",\n        \"expiring_service_token_alert\",\n        \"secondary_dns_all_primaries_failing\",\n        \"secondary_dns_zone_successfully_updated\",\n        \"secondary_dns_zone_validation_warning\",\n        \"sentinel_alert\",\n        \"traffic_anomalies_alert\",\n        \"tunnel_health_event\"\n      ]\n    },\n    \"alert_correlation_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\
  ,\n      \"description\": \"UUID for grouping related alerts that are part of the same incident.\"\n    },\n    \"alert_event\": {\n      \"type\": \"string\",\n      \"description\": \"The event state indicating whether the alert is starting or ending.\",\n      \"enum\": [\"ALERT_STATE_EVENT_START\", \"ALERT_STATE_EVENT_END\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-notification-webhook-payload-schema.json
tags:
- AI Gateway
- API Gateway
- Artificial Intelligence
- CDN
- Cloud
- Containers
- DDoS Protection
- DNS
- Edge
- Edge Computing
- Object Storage
- Platform
- Real-Time Communication
- Security
- Serverless
- Web Performance
title: Cloudflare Notification Webhook Payload
---
