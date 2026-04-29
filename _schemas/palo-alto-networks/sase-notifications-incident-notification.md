---
description: IncidentNotification schema from SASE Multitenant Notifications
layout: schema
name: IncidentNotification
properties_list:
- description: Unique identifier for this notification delivery.
  name: notificationId
  type: string
- description: Notification type identifier.
  name: type
  type: string
- description: Tenant Service Group identifier indicating which tenant context the incident belongs to.
  name: tsg_id
  type: string
- description: Severity classification of the security incident.
  name: severity
  type: string
- description: Brief title summarizing the incident.
  name: title
  type: string
- description: Detailed description of the incident including affected resources, detection context, and recommended actions.
  name: description
  type: string
- description: Timestamp when the incident was detected.
  name: timestamp
  type: string
- description: Incident category such as threat, policy_violation, anomaly, or data_loss.
  name: category
  type: string
- description: List of resources affected by the incident.
  name: affectedResources
  type: array
- description: Direct link to the incident in the SASE management console.
  name: callbackUrl
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-notifications-incident-notification-schema.json
slug: sase-notifications-incident-notification
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IncidentNotification\",\n  \"description\": \"IncidentNotification schema from SASE Multitenant Notifications\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-notifications-incident-notification-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"notificationId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this notification delivery.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"incident\"\n      ],\n      \"description\": \"Notification type identifier.\"\n    },\n    \"tsg_id\": {\n      \"type\": \"string\",\n      \"description\": \"Tenant Service Group identifier indicating which tenant context the incident belongs to.\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"informational\",\n  \
  \      \"low\",\n        \"medium\",\n        \"high\",\n        \"critical\"\n      ],\n      \"description\": \"Severity classification of the security incident.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Brief title summarizing the incident.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed description of the incident including affected resources, detection context, and recommended actions.\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the incident was detected.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Incident category such as threat, policy_violation, anomaly, or data_loss.\"\n    },\n    \"affectedResources\": {\n      \"type\": \"array\",\n      \"description\": \"List of resources affected by the incident.\",\n      \"items\": {\n        \"type\": \"object\"\
  ,\n        \"properties\": {\n          \"resourceType\": {\n            \"type\": \"string\",\n            \"description\": \"Type of affected resource.\"\n          },\n          \"resourceId\": {\n            \"type\": \"string\",\n            \"description\": \"Identifier of the affected resource.\"\n          }\n        }\n      }\n    },\n    \"callbackUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Direct link to the incident in the SASE management console.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-notifications-incident-notification-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: IncidentNotification
---
