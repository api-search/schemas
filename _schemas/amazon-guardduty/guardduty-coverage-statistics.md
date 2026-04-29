---
description: Information about the coverage statistics for a resource.
layout: schema
name: CoverageStatistics
properties_list:
- description: ''
  name: CountByResourceType
  type: object
- description: ''
  name: CountByCoverageStatus
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-coverage-statistics-schema.json
slug: guardduty-coverage-statistics
source_filename: guardduty-coverage-statistics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-coverage-statistics-schema.json\",\n  \"title\": \"CoverageStatistics\",\n  \"description\": \"Information about the coverage statistics for a resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CountByResourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CountByResourceType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"countByResourceType\"\n          },\n          \"description\": \"Represents coverage statistics for EKS clusters aggregated by resource type.\"\n        }\n      ]\n    },\n    \"CountByCoverageStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CountByCoverageStatus\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"countByCoverageStatus\"\n\
  \          },\n          \"description\": \"Represents coverage statistics for EKS clusters aggregated by coverage status.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-coverage-statistics-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: CoverageStatistics
---
