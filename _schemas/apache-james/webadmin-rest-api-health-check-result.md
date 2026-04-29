---
description: Health check results for all components
layout: schema
name: HealthCheckResult
properties_list:
- description: Overall health status
  name: status
  type: string
- description: Individual component checks
  name: checks
  type: array
provider_name: Apache James
provider_slug: apache-james
schema_file: json-schema/webadmin-rest-api-health-check-result-schema.json
slug: webadmin-rest-api-health-check-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/json-schema/webadmin-rest-api-health-check-result-schema.json\",\n  \"title\": \"HealthCheckResult\",\n  \"description\": \"Health check results for all components\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Overall health status\",\n      \"enum\": [\n        \"healthy\",\n        \"degraded\",\n        \"unhealthy\"\n      ],\n      \"example\": \"healthy\"\n    },\n    \"checks\": {\n      \"type\": \"array\",\n      \"description\": \"Individual component checks\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ComponentCheck\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/json-schema/webadmin-rest-api-health-check-result-schema.json
tags:
- Email
- IMAP
- Java
- JMAP
- Mail Server
- Open Source
- SMTP
title: HealthCheckResult
---
