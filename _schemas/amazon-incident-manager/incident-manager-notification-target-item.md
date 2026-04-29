---
description: The SNS targets that are notified when updates are made to an incident.
layout: schema
name: NotificationTargetItem
properties_list:
- description: ''
  name: snsTopicArn
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-notification-target-item-schema.json
slug: incident-manager-notification-target-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-notification-target-item-schema.json\",\n  \"title\": \"NotificationTargetItem\",\n  \"description\": \"The SNS targets that are notified when updates are made to an incident.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"snsTopicArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the SNS topic.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-notification-target-item-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: NotificationTargetItem
---
