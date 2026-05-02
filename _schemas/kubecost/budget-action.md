---
description: A notification action that triggers when a budget threshold is reached.
layout: schema
name: Kubecost Budget Action
properties_list:
- description: Percentage threshold (0-1) at which the action triggers.
  name: threshold
  type: number
- description: Type of notification channel.
  name: type
  type: string
- description: Target for the notification (email address, webhook URL, etc.).
  name: target
  type: string
provider_name: Kubecost
provider_slug: kubecost
schema_file: json-schema/budget-action.json
slug: budget-action
source_filename: budget-action.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kubecost/blob/main/json-schema/budget-action.json\",\n  \"title\": \"Kubecost Budget Action\",\n  \"description\": \"A notification action that triggers when a budget threshold is reached.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"threshold\": {\n      \"type\": \"number\",\n      \"description\": \"Percentage threshold (0-1) at which the action triggers.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"email\",\n        \"slack\",\n        \"msteams\"\n      ],\n      \"description\": \"Type of notification channel.\"\n    },\n    \"target\": {\n      \"type\": \"string\",\n      \"description\": \"Target for the notification (email address, webhook URL, etc.).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kubecost/refs/heads/main/json-schema/budget-action.json
tags:
- Cloud Cost
- Cost Monitoring
- Kubernetes
- Optimization
- Spending
title: Kubecost Budget Action
---
