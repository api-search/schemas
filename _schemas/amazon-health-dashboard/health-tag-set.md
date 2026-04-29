---
description: tagSet schema from Amazon Health Dashboard API
layout: schema
name: tagSet
properties_list: []
provider_name: Amazon Health Dashboard
provider_slug: amazon-health-dashboard
schema_file: json-schema/health-tag-set-schema.json
slug: health-tag-set
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-tag-set-schema.json\",\n  \"title\": \"tagSet\",\n  \"description\": \"tagSet schema from Amazon Health Dashboard API\",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"$ref\": \"#/components/schemas/tagValue\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-health-dashboard/refs/heads/main/json-schema/health-tag-set-schema.json
tags:
- AWS
- Health Monitoring
- Notifications
- Operations
- Service Status
title: tagSet
---
