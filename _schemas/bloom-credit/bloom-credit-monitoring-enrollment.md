---
description: Credit monitoring enrollment record for a consumer.
layout: schema
name: MonitoringEnrollment
properties_list:
- description: Unique identifier for the monitoring enrollment.
  name: enrollment_id
  type: string
- description: Consumer this enrollment belongs to.
  name: consumer_id
  type: string
- description: Enrollment status.
  name: status
  type: string
- description: Bureaus being monitored.
  name: bureaus
  type: array
- description: ''
  name: created_at
  type: string
provider_name: Bloom Credit
provider_slug: bloom-credit
schema_file: json-schema/bloom-credit-monitoring-enrollment-schema.json
slug: bloom-credit-monitoring-enrollment
source_filename: bloom-credit-monitoring-enrollment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bloom-credit/main/json-schema/bloom-credit-monitoring-enrollment-schema.json\",\n  \"title\": \"MonitoringEnrollment\",\n  \"description\": \"Credit monitoring enrollment record for a consumer.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enrollment_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the monitoring enrollment.\",\n      \"example\": \"mon_4b3c2d1e0f9a\"\n    },\n    \"consumer_id\": {\n      \"type\": \"string\",\n      \"description\": \"Consumer this enrollment belongs to.\",\n      \"example\": \"cns_8f7d3a2b1c4e5f6a\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Enrollment status.\",\n      \"enum\": [\"ACTIVE\", \"INACTIVE\", \"PAUSED\"],\n      \"example\": \"ACTIVE\"\n    },\n    \"bureaus\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"Bureaus being monitored.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"equifax\", \"experian\", \"transunion\"]\n      },\n      \"example\": [\"equifax\", \"experian\", \"transunion\"]\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:10:00Z\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloom-credit/refs/heads/main/json-schema/bloom-credit-monitoring-enrollment-schema.json
tags:
- Credit Bureau
- Credit Reports
- Credit Scores
- Fintech
- Lending
- Personal Finance
title: MonitoringEnrollment
---
