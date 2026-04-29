---
description: EventList schema from Amazon Health Dashboard API
layout: schema
name: EventList
properties_list: []
provider_name: Amazon Health Dashboard
provider_slug: amazon-health-dashboard
schema_file: json-schema/health-event-list-schema.json
slug: health-event-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-event-list-schema.json\",\n  \"title\": \"EventList\",\n  \"description\": \"EventList schema from Amazon Health Dashboard API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/Event\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-event-list-schema.json
tags:
- AWS
- Health Monitoring
- Notifications
- Operations
- Service Status
title: EventList
---
