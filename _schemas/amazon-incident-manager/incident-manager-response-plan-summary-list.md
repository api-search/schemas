---
description: ResponsePlanSummaryList schema
layout: schema
name: ResponsePlanSummaryList
properties_list: []
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-response-plan-summary-list-schema.json
slug: incident-manager-response-plan-summary-list
source_filename: incident-manager-response-plan-summary-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-response-plan-summary-list-schema.json\",\n  \"title\": \"ResponsePlanSummaryList\",\n  \"description\": \"ResponsePlanSummaryList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"arn\",\n      \"name\"\n    ],\n    \"properties\": {\n      \"arn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Arn\"\n          },\n          {\n            \"description\": \"The Amazon Resource Name (ARN) of the response plan.\"\n          }\n        ]\n      },\n      \"displayName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ResponsePlanDisplayName\"\n          },\n          {\n            \"description\": \"The human readable name of the response plan. This\
  \ can include spaces.\"\n          }\n        ]\n      },\n      \"name\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ResponsePlanName\"\n          },\n          {\n            \"description\": \"The name of the response plan. This can't include spaces.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Details of the response plan that are used when creating an incident.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-response-plan-summary-list-schema.json
tags:
- Automation
- DevOps
- Incident Management
- Operations
title: ResponsePlanSummaryList
---
