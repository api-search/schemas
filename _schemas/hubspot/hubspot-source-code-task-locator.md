---
description: Locator for an asynchronous task
layout: schema
name: TaskLocator
properties_list:
- description: Unique identifier for the task
  name: id
  type: string
- description: Related links for the task
  name: links
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-source-code-task-locator-schema.json
slug: hubspot-source-code-task-locator
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Locator for an asynchronous task\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the task\",\n      \"example\": \"12345\"\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"description\": \"Related links for the task\",\n      \"example\": {\n        \"status\": \"/cms/v3/source-code/extract/async/tasks/12345/status\"\n      }\n    }\n  },\n  \"required\": [\n    \"id\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TaskLocator\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-source-code-task-locator-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: TaskLocator
---
