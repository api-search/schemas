---
description: Health check result for a single component
layout: schema
name: ComponentCheck
properties_list:
- description: Component name
  name: componentName
  type: string
- description: URL-encoded component name
  name: escapedComponentName
  type: string
- description: Component health status
  name: status
  type: string
- description: Reason for unhealthy status (if applicable)
  name: cause
  type: string
provider_name: Apache James
provider_slug: apache-james
schema_file: json-schema/webadmin-rest-api-component-check-schema.json
slug: webadmin-rest-api-component-check
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/json-schema/webadmin-rest-api-component-check-schema.json\",\n  \"title\": \"ComponentCheck\",\n  \"description\": \"Health check result for a single component\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"componentName\": {\n      \"type\": \"string\",\n      \"description\": \"Component name\",\n      \"example\": \"Cassandra backend\"\n    },\n    \"escapedComponentName\": {\n      \"type\": \"string\",\n      \"description\": \"URL-encoded component name\",\n      \"example\": \"Cassandra%20backend\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Component health status\",\n      \"enum\": [\n        \"healthy\",\n        \"degraded\",\n        \"unhealthy\"\n      ],\n      \"example\": \"healthy\"\n    },\n    \"cause\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Reason for unhealthy status (if applicable)\",\n      \"example\": \"Connection timeout\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/json-schema/webadmin-rest-api-component-check-schema.json
tags:
- Email
- IMAP
- Java
- JMAP
- Mail Server
- Open Source
- SMTP
title: ComponentCheck
---
