---
description: Information about the number of open reactive and proactive insights that can be used to gauge the health of your system.
layout: schema
name: InsightHealth
properties_list:
- description: ''
  name: OpenProactiveInsights
  type: object
- description: ''
  name: OpenReactiveInsights
  type: object
- description: ''
  name: MeanTimeToRecoverInMilliseconds
  type: object
provider_name: Amazon DevOps Guru
provider_slug: amazon-devops-guru
schema_file: json-schema/amazon-devops-guru-insight-health-schema.json
slug: amazon-devops-guru-insight-health
source_filename: amazon-devops-guru-insight-health-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-insight-health-schema.json\",\n  \"title\": \"InsightHealth\",\n  \"description\": \"Information about the number of open reactive and proactive insights that can be used to gauge the health of your system.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OpenProactiveInsights\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NumOpenProactiveInsights\"\n        },\n        {\n          \"description\": \" The number of open proactive insights. \"\n        }\n      ]\n    },\n    \"OpenReactiveInsights\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NumOpenReactiveInsights\"\n        },\n        {\n          \"description\": \" The number of open reactive insights. \"\n        }\n      ]\n    },\n    \"MeanTimeToRecoverInMilliseconds\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MeanTimeToRecoverInMilliseconds\"\n        },\n        {\n          \"description\": \" The Meant Time to Recover (MTTR) for the insight. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-insight-health-schema.json
tags:
- Anomaly Detection
- DevOps
- Machine Learning
- Operational Intelligence
title: InsightHealth
---
