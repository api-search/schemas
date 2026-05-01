---
description: CreateDeploymentResponse schema from AWS Mainframe Modernization API
layout: schema
name: CreateDeploymentResponse
properties_list:
- description: ''
  name: deploymentId
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-create-deployment-response-schema.json
slug: amazon-mainframe-modernization-create-deployment-response
source_filename: amazon-mainframe-modernization-create-deployment-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-create-deployment-response-schema.json\",\n  \"title\": \"CreateDeploymentResponse\",\n  \"description\": \"CreateDeploymentResponse schema from AWS Mainframe Modernization API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Identifier\"\n        },\n        {\n          \"description\": \"The unique identifier of the deployment.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"deploymentId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-create-deployment-response-schema.json
tags:
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: CreateDeploymentResponse
---
