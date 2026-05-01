---
description: Represents the health of an Amazon Web Services service.
layout: schema
name: ServiceHealth
properties_list:
- description: ''
  name: ServiceName
  type: object
- description: ''
  name: Insight
  type: object
- description: ''
  name: AnalyzedResourceCount
  type: object
provider_name: Amazon DevOps Guru
provider_slug: amazon-devops-guru
schema_file: json-schema/amazon-devops-guru-service-health-schema.json
slug: amazon-devops-guru-service-health
source_filename: amazon-devops-guru-service-health-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-service-health-schema.json\",\n  \"title\": \"ServiceHealth\",\n  \"description\": \"Represents the health of an Amazon Web Services service.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ServiceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceName\"\n        },\n        {\n          \"description\": \"The name of the Amazon Web Services service.\"\n        }\n      ]\n    },\n    \"Insight\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceInsightHealth\"\n        },\n        {\n          \"description\": \"Represents the health of an Amazon Web Services service. This is a <code>ServiceInsightHealth</code> that contains the number of open proactive and reactive insights for this service.\"\n\
  \        }\n      ]\n    },\n    \"AnalyzedResourceCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnalyzedResourceCount\"\n        },\n        {\n          \"description\": \" Number of resources that DevOps Guru is monitoring in an analyzed Amazon Web Services service. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-service-health-schema.json
tags:
- Anomaly Detection
- DevOps
- Machine Learning
- Operational Intelligence
title: ServiceHealth
---
