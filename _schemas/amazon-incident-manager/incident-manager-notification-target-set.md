---
description: NotificationTargetSet schema
layout: schema
name: NotificationTargetSet
properties_list: []
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-notification-target-set-schema.json
slug: incident-manager-notification-target-set
source_filename: incident-manager-notification-target-set-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-notification-target-set-schema.json\",\n  \"title\": \"NotificationTargetSet\",\n  \"description\": \"NotificationTargetSet schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"snsTopicArn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Arn\"\n          },\n          {\n            \"description\": \"The Amazon Resource Name (ARN) of the SNS topic.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"The SNS targets that are notified when updates are made to an incident.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-notification-target-set-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: NotificationTargetSet
---
