---
description: Information about the health of Amazon Web Services resources in your account that are specified by an Amazon Web Services CloudFormation stack.
layout: schema
name: CloudFormationHealth
properties_list:
- description: ''
  name: StackName
  type: object
- description: ''
  name: Insight
  type: object
- description: ''
  name: AnalyzedResourceCount
  type: object
provider_name: Amazon DevOps Guru
provider_slug: amazon-devops-guru
schema_file: json-schema/amazon-devops-guru-cloud-formation-health-schema.json
slug: amazon-devops-guru-cloud-formation-health
source_filename: amazon-devops-guru-cloud-formation-health-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-cloud-formation-health-schema.json\",\n  \"title\": \"CloudFormationHealth\",\n  \"description\": \"Information about the health of Amazon Web Services resources in your account that are specified by an Amazon Web Services CloudFormation stack.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StackName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StackName\"\n        },\n        {\n          \"description\": \" The name of the CloudFormation stack. \"\n        }\n      ]\n    },\n    \"Insight\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InsightHealth\"\n        },\n        {\n          \"description\": \" Information about the health of the Amazon Web Services resources in your account that are specified\
  \ by an Amazon Web Services CloudFormation stack, including the number of open proactive, open reactive insights, and the Mean Time to Recover (MTTR) of closed insights. \"\n        }\n      ]\n    },\n    \"AnalyzedResourceCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnalyzedResourceCount\"\n        },\n        {\n          \"description\": \" Number of resources that DevOps Guru is monitoring in your account that are specified by an Amazon Web Services CloudFormation stack. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-cloud-formation-health-schema.json
tags:
- Anomaly Detection
- DevOps
- Machine Learning
- Operational Intelligence
title: CloudFormationHealth
---
