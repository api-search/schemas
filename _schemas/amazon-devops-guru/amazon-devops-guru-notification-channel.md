---
description: Information about a notification channel. A notification channel is used to notify you when DevOps Guru creates an insight. The one supported notification channel is Amazon Simple Notification Service (Amazon SNS). If you use an Amazon SNS topic in another account, you must attach a policy to it th
layout: schema
name: NotificationChannel
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: Config
  type: object
provider_name: Amazon DevOps Guru
provider_slug: amazon-devops-guru
schema_file: json-schema/amazon-devops-guru-notification-channel-schema.json
slug: amazon-devops-guru-notification-channel
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-notification-channel-schema.json\",\n  \"title\": \"NotificationChannel\",\n  \"description\": \"Information about a notification channel. A notification channel is used to notify you when DevOps Guru creates an insight. The one supported notification channel is Amazon Simple Notification Service (Amazon SNS).  If you use an Amazon SNS topic in another account, you must attach a policy to it th\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotificationChannelId\"\n        },\n        {\n          \"description\": \" The ID of a notification channel. \"\n        }\n      ]\n    },\n    \"Config\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotificationChannelConfig\"\
  \n        },\n        {\n          \"description\": \" A <code>NotificationChannelConfig</code> object that contains information about configured notification channels. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-notification-channel-schema.json
tags:
- Anomaly Detection
- AWS
- DevOps
- Machine Learning
- Operational Intelligence
title: NotificationChannel
---
