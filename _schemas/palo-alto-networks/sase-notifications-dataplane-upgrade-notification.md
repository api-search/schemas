---
description: DataplaneUpgradeNotification schema from SASE Multitenant Notifications
layout: schema
name: DataplaneUpgradeNotification
properties_list:
- description: Unique identifier for this notification delivery.
  name: notificationId
  type: string
- description: Notification type identifier.
  name: type
  type: string
- description: Tenant Service Group identifier for the affected tenant.
  name: tsg_id
  type: string
- description: SASE compute region where the dataplane upgrade is occurring, such as us-east-1, eu-west-1, or ap-southeast-1.
  name: region
  type: string
- description: Current dataplane software version before the upgrade.
  name: currentVersion
  type: string
- description: Target dataplane software version after the upgrade completes.
  name: targetVersion
  type: string
- description: Scheduled start time for the dataplane upgrade maintenance window.
  name: scheduledTime
  type: string
- description: Estimated end time for the dataplane upgrade maintenance window.
  name: estimatedEndTime
  type: string
- description: Current status of the dataplane upgrade.
  name: status
  type: string
- description: Timestamp when this notification was generated.
  name: timestamp
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-notifications-dataplane-upgrade-notification-schema.json
slug: sase-notifications-dataplane-upgrade-notification
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataplaneUpgradeNotification\",\n  \"description\": \"DataplaneUpgradeNotification schema from SASE Multitenant Notifications\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-notifications-dataplane-upgrade-notification-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"notificationId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this notification delivery.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"dataplane_upgrade\"\n      ],\n      \"description\": \"Notification type identifier.\"\n    },\n    \"tsg_id\": {\n      \"type\": \"string\",\n      \"description\": \"Tenant Service Group identifier for the affected tenant.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"SASE compute region where\
  \ the dataplane upgrade is occurring, such as us-east-1, eu-west-1, or ap-southeast-1.\"\n    },\n    \"currentVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Current dataplane software version before the upgrade.\"\n    },\n    \"targetVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Target dataplane software version after the upgrade completes.\"\n    },\n    \"scheduledTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Scheduled start time for the dataplane upgrade maintenance window.\"\n    },\n    \"estimatedEndTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Estimated end time for the dataplane upgrade maintenance window.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"scheduled\",\n        \"in_progress\",\n        \"completed\",\n        \"failed\",\n        \"rolled_back\"\n      ],\n      \"description\"\
  : \"Current status of the dataplane upgrade.\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when this notification was generated.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-notifications-dataplane-upgrade-notification-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: DataplaneUpgradeNotification
---
