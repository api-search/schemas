---
description: Contains information about finding statistics.
layout: schema
name: FindingStatistics
properties_list:
- description: ''
  name: CountBySeverity
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-finding-statistics-schema.json
slug: guardduty-finding-statistics
source_filename: guardduty-finding-statistics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-finding-statistics-schema.json\",\n  \"title\": \"FindingStatistics\",\n  \"description\": \"Contains information about finding statistics.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CountBySeverity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CountBySeverity\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"countBySeverity\"\n          },\n          \"description\": \"Represents a map of severity to count statistics for a set of findings.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-finding-statistics-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: FindingStatistics
---
