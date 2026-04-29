---
description: List of maintenance plans.
layout: schema
name: MaintenancePlansResponse
properties_list:
- description: Array of maintenance plans.
  name: maintenance_plans
  type: array
provider_name: BigPanda
provider_slug: bigpanda
schema_file: json-schema/bigpanda-maintenance-plans-response-schema.json
slug: bigpanda-maintenance-plans-response
source_filename: bigpanda-maintenance-plans-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"MaintenancePlansResponse\",\n  \"type\": \"object\",\n  \"description\": \"List of maintenance plans.\",\n  \"properties\": {\n    \"maintenance_plans\": {\n      \"type\": \"array\",\n      \"description\": \"Array of maintenance plans.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MaintenancePlan\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bigpanda/refs/heads/main/json-schema/bigpanda-maintenance-plans-response-schema.json
tags:
- Incidents
- Monitoring
- Platform
title: MaintenancePlansResponse
---
