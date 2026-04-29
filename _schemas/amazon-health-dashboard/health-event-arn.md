---
description: eventArn schema from Amazon Health Dashboard API
layout: schema
name: eventArn
properties_list: []
provider_name: Amazon Health Dashboard
provider_slug: amazon-health-dashboard
schema_file: json-schema/health-event-arn-schema.json
slug: health-event-arn
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-event-arn-schema.json\",\n  \"title\": \"eventArn\",\n  \"description\": \"eventArn schema from Amazon Health Dashboard API\",\n  \"type\": \"string\",\n  \"pattern\": \"arn:aws(-[a-z]+(-[a-z]+)?)?:health:[^:]*:[^:]*:event(?:/[\\\\w-]+){3}\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-event-arn-schema.json
tags:
- AWS
- Health Monitoring
- Notifications
- Operations
- Service Status
title: eventArn
---
