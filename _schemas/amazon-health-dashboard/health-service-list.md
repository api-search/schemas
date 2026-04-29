---
description: serviceList schema from Amazon Health Dashboard API
layout: schema
name: serviceList
properties_list: []
provider_name: Amazon Health Dashboard
provider_slug: amazon-health-dashboard
schema_file: json-schema/health-service-list-schema.json
slug: health-service-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-service-list-schema.json\",\n  \"title\": \"serviceList\",\n  \"description\": \"serviceList schema from Amazon Health Dashboard API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/service\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-service-list-schema.json
tags:
- AWS
- Health Monitoring
- Notifications
- Operations
- Service Status
title: serviceList
---
