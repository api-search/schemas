---
description: EngagementSet schema
layout: schema
name: EngagementSet
properties_list: []
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-engagement-set-schema.json
slug: incident-manager-engagement-set
source_filename: incident-manager-engagement-set-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-engagement-set-schema.json\",\n  \"title\": \"EngagementSet\",\n  \"description\": \"EngagementSet schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"pattern\": \"^arn:aws(-cn|-us-gov)?:ssm-contacts:[a-z0-9-]*:([0-9]{12}):contact/[a-z0-9_-]+$\",\n    \"minLength\": 0,\n    \"maxLength\": 2048\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-engagement-set-schema.json
tags:
- Automation
- DevOps
- Incident Management
- Operations
title: EngagementSet
---
