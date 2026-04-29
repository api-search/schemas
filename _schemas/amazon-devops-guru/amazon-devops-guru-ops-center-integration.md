---
description: Information about whether DevOps Guru is configured to create an OpsItem in Amazon Web Services Systems Manager OpsCenter for each created insight.
layout: schema
name: OpsCenterIntegration
properties_list:
- description: ''
  name: OptInStatus
  type: object
provider_name: Amazon DevOps Guru
provider_slug: amazon-devops-guru
schema_file: json-schema/amazon-devops-guru-ops-center-integration-schema.json
slug: amazon-devops-guru-ops-center-integration
source_filename: amazon-devops-guru-ops-center-integration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-ops-center-integration-schema.json\",\n  \"title\": \"OpsCenterIntegration\",\n  \"description\": \"Information about whether DevOps Guru is configured to create an OpsItem in Amazon Web Services Systems Manager OpsCenter for each created insight.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OptInStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OptInStatus\"\n        },\n        {\n          \"description\": \" Specifies if DevOps Guru is enabled to create an Amazon Web Services Systems Manager OpsItem for each created insight. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-ops-center-integration-schema.json
tags:
- Anomaly Detection
- AWS
- DevOps
- Machine Learning
- Operational Intelligence
title: OpsCenterIntegration
---
