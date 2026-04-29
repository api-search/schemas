---
description: AnnouncementNotification schema from SASE Multitenant Notifications
layout: schema
name: AnnouncementNotification
properties_list:
- description: Unique identifier for this notification delivery.
  name: notificationId
  type: string
- description: Notification type identifier.
  name: type
  type: string
- description: Announcement title.
  name: title
  type: string
- description: Full announcement body with details about the platform change, maintenance window, or service update.
  name: body
  type: string
- description: Category of the announcement.
  name: category
  type: string
- description: List of SASE services affected by the announcement, such as Prisma Access, GlobalProtect, ADEM, SWG, or ZTNA.
  name: affectedServices
  type: array
- description: Date and time when the announced change takes effect.
  name: effectiveDate
  type: string
- description: Timestamp when the announcement was published.
  name: timestamp
  type: string
- description: Tenant Service Group identifier if the announcement is tenant-specific. Omitted for global announcements.
  name: tsg_id
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-notifications-announcement-notification-schema.json
slug: sase-notifications-announcement-notification
source_filename: sase-notifications-announcement-notification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AnnouncementNotification\",\n  \"description\": \"AnnouncementNotification schema from SASE Multitenant Notifications\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-notifications-announcement-notification-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"notificationId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this notification delivery.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"announcement\"\n      ],\n      \"description\": \"Notification type identifier.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Announcement title.\"\n    },\n    \"body\": {\n      \"type\": \"string\",\n      \"description\": \"Full announcement body with details about the platform change, maintenance window,\
  \ or service update.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"maintenance\",\n        \"feature_release\",\n        \"deprecation\",\n        \"service_status\",\n        \"security_advisory\"\n      ],\n      \"description\": \"Category of the announcement.\"\n    },\n    \"affectedServices\": {\n      \"type\": \"array\",\n      \"description\": \"List of SASE services affected by the announcement, such as Prisma Access, GlobalProtect, ADEM, SWG, or ZTNA.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when the announced change takes effect.\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the announcement was published.\"\n    },\n    \"tsg_id\": {\n      \"type\": \"string\",\n      \"description\":\
  \ \"Tenant Service Group identifier if the announcement is tenant-specific. Omitted for global announcements.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-notifications-announcement-notification-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: AnnouncementNotification
---
