---
description: Contains the number of open proactive and reactive insights in an analyzed Amazon Web Services service.
layout: schema
name: ServiceInsightHealth
properties_list:
- description: ''
  name: OpenProactiveInsights
  type: object
- description: ''
  name: OpenReactiveInsights
  type: object
provider_name: Amazon DevOps Guru
provider_slug: amazon-devops-guru
schema_file: json-schema/amazon-devops-guru-service-insight-health-schema.json
slug: amazon-devops-guru-service-insight-health
source_filename: amazon-devops-guru-service-insight-health-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-service-insight-health-schema.json\",\n  \"title\": \"ServiceInsightHealth\",\n  \"description\": \"Contains the number of open proactive and reactive insights in an analyzed Amazon Web Services service.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OpenProactiveInsights\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NumOpenProactiveInsights\"\n        },\n        {\n          \"description\": \"The number of open proactive insights in the Amazon Web Services service\"\n        }\n      ]\n    },\n    \"OpenReactiveInsights\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NumOpenReactiveInsights\"\n        },\n        {\n          \"description\": \"The number of open reactive insights in the Amazon Web Services\
  \ service\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-service-insight-health-schema.json
tags:
- Anomaly Detection
- DevOps
- Machine Learning
- Operational Intelligence
title: ServiceInsightHealth
---
