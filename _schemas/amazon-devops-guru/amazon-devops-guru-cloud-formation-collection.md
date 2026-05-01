---
description: Information about Amazon Web Services CloudFormation stacks. You can use up to 500 stacks to specify which Amazon Web Services resources in your account to analyze. For more information, see Stacks in the Amazon Web Services CloudFormation User Guide.
layout: schema
name: CloudFormationCollection
properties_list:
- description: ''
  name: StackNames
  type: object
provider_name: Amazon DevOps Guru
provider_slug: amazon-devops-guru
schema_file: json-schema/amazon-devops-guru-cloud-formation-collection-schema.json
slug: amazon-devops-guru-cloud-formation-collection
source_filename: amazon-devops-guru-cloud-formation-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-cloud-formation-collection-schema.json\",\n  \"title\": \"CloudFormationCollection\",\n  \"description\": \"Information about Amazon Web Services CloudFormation stacks. You can use up to 500 stacks to specify which Amazon Web Services resources in your account to analyze. For more information, see Stacks in the Amazon Web Services CloudFormation User Guide.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StackNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StackNames\"\n        },\n        {\n          \"description\": \" An array of CloudFormation stack names. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-cloud-formation-collection-schema.json
tags:
- Anomaly Detection
- DevOps
- Machine Learning
- Operational Intelligence
title: CloudFormationCollection
---
